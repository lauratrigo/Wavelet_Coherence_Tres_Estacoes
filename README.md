# 🌐 Coerência Wavelet Ionosfera × Elétricos – Três Estações – Agosto 2017

Este repositório contém scripts MATLAB para calcular a **Coerência Wavelet Contínua (WCOH)** entre parâmetros **ionosféricos** e **elétricos (PPEF, DDEF)** nas estações:

- **Araguatins (ARG)**
- **São José dos Campos (SJC)**
- **Jataí (JAT)**

durante **agosto de 2017**. O objetivo é investigar o acoplamento espectral entre a ionosfera e perturbações eletrodinâmicas.

---

## 🛠 Tecnologias Usadas

- **MATLAB (R2019b ou superior)**
- **Wavelet Toolbox**
- Arquivos `.mat` com parâmetros ionosféricos (5 min)
- Arquivo `drift.dat` com parâmetros elétricos (15 min)

![MATLAB Badge](https://img.shields.io/badge/MATLAB-R2019b-orange?logo=Mathworks&logoColor=white)

---

## 📊 Dados Utilizados

- **Parâmetros Ionosféricos (5 min)**: `foF2`, `hF`, `hmF2`
- **Parâmetros Elétricos (15 min)**: `PPEF`, `DDEF`

---

💡 Objetivo

- Aplicar análise de **coerência wavelet contínua (WCOH)** para identificar padrões espectro-temporais e períodos dominantes em séries temporais de parâmetros **ionosféricos** (`foF2`, `hF`, `hmF2`) e **elétricos** (`PPEF`, `DDEF`) medidos nas estações **Araguatins (ARG)**, **São José dos Campos (SJC)** e **Jataí (JAT)** durante **agosto de 2017**.

---

## 📂 Estrutura do Projeto

```
wcoh_3estacoes/
├── dados/
│ ├── mediasionosfericasARG.mat
│ ├── mediasionosfericasSJC.mat
│ ├── mediasionosfericasJAT.mat
│ └── drift.dat
├── images/
│ ├── WCOH_ARG_foF2_PPEF.png
│ ├── WCOH_ARG_hmF2_DDEF.png
│ ├── WCOH_SJC_hF_PPEF.png
│ ├── WCOH_JAT_foF2_DDEF.png
│ └── ...
├── wav_fejer_arg_sem_vd.m
├── wav_fejer_sjc_sem_vd.m
├── wav_fejer_jat_sem_vd.m
└── README.md
```

---

## ⚙️ Como Executar

---

## ⚙️ Como Executar

1. Clone o repositório:

```bash
git clone https://github.com/lauratrigo/Wavelet_Coherence_3Estacoes.git
cd wcoh_3estacoes
```

2. Abra o MATLAB, certifique-se de que os arquivos .mat e drift.dat estão na pasta dados/.

3. Execute:
   
```bash
run wav_fejer_arg_sem_vd.m   % Araguatins (ARG)
run wav_fejer_sjc_sem_vd.m   % São José dos Campos (SJC)
run wav_fejer_jat_sem_vd.m   % Jataí (JAT)
```

Os gráficos serão salvos em images/.

## 📈 Gráficos Gerados

### Araguatins (ARG)

<!-- h'F -->
<div align="center">
  <h4><strong>h'F × PPEF</strong></h4>
  <img src="images/WCOH_ARG_hF_PPEF.png" alt="WCOH h'F × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>h'F × DDEF</strong></h4>
  <img src="images/WCOH_ARG_hF_DDEF.png" alt="WCOH h'F × DDEF" style="width:80%; max-width:900px;">
</div>

<!-- hmF2 -->
<div align="center">
  <h4><strong>hmF2 × PPEF</strong></h4>
  <img src="images/WCOH_ARG_hmF2_PPEF.png" alt="WCOH hmF2 × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>hmF2 × DDEF</strong></h4>
  <img src="images/WCOH_ARG_hmF2_DDEF.png" alt="WCOH hmF2 × DDEF" style="width:80%; max-width:900px;">
</div>

<!-- foF2 -->
<div align="center">
  <h4><strong>foF2 × PPEF</strong></h4>
  <img src="images/WCOH_ARG_foF2_PPEF.png" alt="WCOH foF2 × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>foF2 × DDEF</strong></h4>
  <img src="images/WCOH_ARG_foF2_DDEF.png" alt="WCOH foF2 × DDEF" style="width:80%; max-width:900px;">
</div>

---

### São José dos Campos (SJC)

<!-- h'F -->
<div align="center">
  <h4><strong>h'F × PPEF</strong></h4>
  <img src="images/WCOH_SJC_hF_PPEF.png" alt="WCOH h'F × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>h'F × DDEF</strong></h4>
  <img src="images/WCOH_SJC_hF_DDEF.png" alt="WCOH h'F × DDEF" style="width:80%; max-width:900px;">
</div>

<!-- hmF2 -->
<div align="center">
  <h4><strong>hmF2 × PPEF</strong></h4>
  <img src="images/WCOH_SJC_hmF2_PPEF.png" alt="WCOH hmF2 × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>hmF2 × DDEF</strong></h4>
  <img src="images/WCOH_SJC_hmF2_DDEF.png" alt="WCOH hmF2 × DDEF" style="width:80%; max-width:900px;">
</div>

<!-- foF2 -->
<div align="center">
  <h4><strong>foF2 × PPEF</strong></h4>
  <img src="images/WCOH_SJC_foF2_PPEF.png" alt="WCOH foF2 × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>foF2 × DDEF</strong></h4>
  <img src="images/WCOH_SJC_foF2_DDEF.png" alt="WCOH foF2 × DDEF" style="width:80%; max-width:900px;">
</div>

---

### Jataí (JAT)

<!-- h'F -->
<div align="center">
  <h4><strong>h'F × PPEF</strong></h4>
  <img src="images/WCOH_JAT_hF_PPEF.png" alt="WCOH h'F × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>h'F × DDEF</strong></h4>
  <img src="images/WCOH_JAT_hF_DDEF.png" alt="WCOH h'F × DDEF" style="width:80%; max-width:900px;">
</div>

<!-- hmF2 -->
<div align="center">
  <h4><strong>hmF2 × PPEF</strong></h4>
  <img src="images/WCOH_JAT_hmF2_PPEF.png" alt="WCOH hmF2 × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>hmF2 × DDEF</strong></h4>
  <img src="images/WCOH_JAT_hmF2_DDEF.png" alt="WCOH hmF2 × DDEF" style="width:80%; max-width:900px;">
</div>

<!-- foF2 -->
<div align="center">
  <h4><strong>foF2 × PPEF</strong></h4>
  <img src="images/WCOH_JAT_foF2_PPEF.png" alt="WCOH foF2 × PPEF" style="width:80%; max-width:900px;">
</div>
<div align="center">
  <h4><strong>foF2 × DDEF</strong></h4>
  <img src="images/WCOH_JAT_foF2_DDEF.png" alt="WCOH foF2 × DDEF" style="width:80%; max-width:900px;">
</div>

---

## 🤝 Agradecimentos

Este projeto foi desenvolvido como parte de um trabalho de pesquisa em Física Espacial no IP&D/UNIVAP, com apoio do grupo de estudos em ionosfera e geomagnetismo.

---

## 📜 Licença

Este repositório está licenciado sob MIT License. Consulte o arquivo LICENSE para mais informações.
