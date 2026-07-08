# Segregação Socioespacial, Saneamento Básico e Racismo Ambiental em Niterói (RJ)

Repositório contendo os códigos, dados e procedimentos utilizados na elaboração do artigo:

> **Segregação Socioespacial, Saneamento Básico e Racismo Ambiental em Niterói-RJ**

O objetivo deste repositório é disponibilizar os scripts utilizados na construção dos indicadores, análises estatísticas e figuras apresentadas no artigo, promovendo transparência e reprodutibilidade científica.

---

# Objetivos

O estudo investiga a relação entre:

- composição racial;
- renda domiciliar;
- acesso ao saneamento básico;

utilizando dados do Censo Demográfico de 2010 (IBGE), tendo como unidade espacial os setores censitários do município de Niterói (RJ).

Como medida sintética das condições de saneamento foi desenvolvido o **Índice E.L.A.**, composto pelos indicadores de:

- Esgotamento Sanitário;
- Coleta de Resíduos Sólidos;
- Abastecimento de Água.

Também são realizadas análises de regressão linear múltipla (OLS) e regressão quantílica para avaliar a influência da renda e da composição racial sobre o índice.

---

# Estrutura do repositório

```
├── dados/
│   ├── IBGE/
│   ├── shapefiles/
│   ├── tabelas/
│
├── notebooks/
│   ├── Memorial_de_Calculo.ipynb
│
├── figuras/
│
├── scripts/
│
├── README.md
```

---

# Fluxo da análise

O processamento segue as seguintes etapas:

1. Importação das bases do IBGE;
2. Limpeza e tratamento dos dados;
3. Cálculo dos indicadores de saneamento;
4. Construção do Índice E.L.A.;
5. Classificação dos setores censitários;
6. Geração dos gráficos;
7. Regressão Linear (OLS);
8. Regressão Quantílica;
9. Exportação das figuras utilizadas no artigo.

---

# Índice E.L.A.

O Índice E.L.A. representa a média aritmética simples dos três indicadores de saneamento:

- Esgotamento Sanitário
- Coleta de Lixo
- Abastecimento de Água

Valores próximos de **100** representam melhor cobertura dos serviços básicos.

---

# Bibliotecas utilizadas

- pandas
- numpy
- matplotlib
- plotly
- statsmodels
- scikit-learn
- scipy

---

# Dados

As análises utilizam principalmente:

- Censo Demográfico 2010 (IBGE)
- Setores censitários
- Bases cartográficas do SiGeo Niterói

Os dados públicos permanecem sob responsabilidade de seus respectivos órgãos.

---

# Reprodução

Clone o repositório:

```bash
git clone https://github.com/usuario/repositorio.git
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

Execute o notebook:

```
notebooks/Memorial_de_Calculo.ipynb
```

---

# Resultados

O notebook gera automaticamente todas as figuras utilizadas no artigo, incluindo:

- distribuição dos indicadores de saneamento;
- boxplots do Índice E.L.A.;
- gráficos de dispersão;
- regressão linear;
- regressão quantílica.

---

# Licença

Este projeto é disponibilizado para fins acadêmicos e científicos.

Caso utilize os códigos ou adaptações deste trabalho, cite o artigo correspondente.

---

# Citação

Caso utilize este material, cite:

> Segregação Socioespacial, Saneamento Básico e Racismo Ambiental em Niterói-RJ.
