# Projeto Final – Ciência de Dados  
## Análise do Dataset: YouTube Posting Dataset

Este repositório contém o desenvolvimento completo do Trabalho Final da disciplina **Ciência de Dados**, abordando a análise exploratória, pré-processamento, consultas, visualizações e conclusões utilizando o dataset *YouTube Posting Dataset*.

---

## 👥 Integrantes do Grupo
- Kauã Henrique Fachin Munchen  
- Beatriz Amanda dos Santos
- Rayana Gabriela Nunes Conrat 

---

## 📌 Descrição do Projeto
O objetivo deste projeto foi realizar uma análise exploratória e extrair insights relevantes sobre vídeos do YouTube, considerando métricas como visualizações, seguidores do canal, categorias e engajamento.  

O dataset utilizado contém informações sobre títulos, categorias, número de visualizações, tamanho do canal e outras características relacionadas ao conteúdo publicado na plataforma.  
As análises foram realizadas utilizando **Python**, em ambiente **Jupyter Notebook (VS Code)**.


## Estrutura do Repositório
├── analysis.ipynb # Notebook completo com todas as etapas
├── Dados.YT.csv # Dataset utilizado 
├── README.md # Este arquivo
└── presentation/ Slides da apresentação

---

## Base de Dados Utilizada
**YouTube Posting Dataset – Kaggle**  
Disponível em:  
https://www.kaggle.com/datasets/grandmaster07/youtube-posting-dataset/data

---

## Tecnologias Utilizadas

- **Python 3.13**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **VS Code + Jupyter Notebook**
- **Git & GitHub**

---

## Etapas do Projeto

### Leitura e Entendimento da Base**
- Carregamento do dataset  
- Verificação de estrutura (`info()`, `describe()`, `head()`)  
- Identificação das colunas presentes  

### Pré-processamento dos Dados**
- Renomeação e padronização de colunas  
- Remoção de duplicados  
- Tratamento de valores nulos  
- Criação de novas métricas:  
  - `Engagement` = Views / Followers  
  - `IsPopular` (popularidade com base na mediana)  
- Normalização textual (título e categoria)

### Consultas e Agrupamentos**
- Categorias mais frequentes  
- Top 10 vídeos mais visualizados  
- Média de visualizações por categoria  
- Engajamento médio por categoria  
- Distribuição de vídeos populares  

### Visualizações Gráficas**
Foram criados gráficos utilizando Matplotlib e Seaborn, incluindo:
- Histograma de visualizações  
- Barra: média de views por categoria  
- Barra: engajamento médio por categoria  
- Boxplot de views por categoria  
- Gráfico de barras: popular vs. não popular  

### Conclusões
- Vídeos seguem distribuição assimétrica (poucos vídeos muito populares)  
- Algumas categorias se destacam significativamente em views  
- Canais pequenos podem ter alto engajamento relativo  
- A métrica `IsPopular` mostrou bom equilíbrio entre classes  
- Ausência de dados temporais limitou análises de tendência  

As conclusões completas estão no final do arquivo *analysis.ipynb*.

---

## Como Executar o Projeto

### 🔧 1. Instale as dependências
No terminal:

```bash
py -m pip install pandas matplotlib seaborn
