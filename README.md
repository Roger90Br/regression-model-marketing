# Análise de Investimentos em Marketing e Previsão de Vendas

Este projeto realiza uma análise dos investimentos em diferentes plataformas de marketing (YouTube, Facebook e jornais) e sua relação com as vendas resultantes. Utiliza-se de técnicas estatísticas e de aprendizado de máquina para explorar os dados e prever o impacto dos investimentos em vendas.

## Objetivos

- Analisar a distribuição dos investimentos em marketing nas plataformas YouTube, Facebook e jornais.
- Explorar a relação entre os investimentos e as vendas.
- Criar um modelo de regressão linear para prever as vendas com base nos investimentos em marketing.

## Estrutura do Projeto

### 1. Carregamento e Preparação dos Dados
Os dados são carregados a partir de um arquivo CSV (`MKT.csv`) utilizando o pandas. A primeira análise consiste na descrição estatística dos dados.

- `describe()` para calcular medidas como média, desvio padrão, mínimo, máximo, etc.
- Exibição dos dados faltantes e tipos de dados.

### 2. Análise Exploratória

#### Descrição dos Dados
A descrição estatística das variáveis (YouTube, Facebook, Newspaper e Sales) é apresentada com valores arredondados para 2 casas decimais.

#### Gráficos

- **Gráfico de Pizza**: Representa a distribuição dos investimentos em marketing por plataforma.
- **Matriz de Correlação**: Analisa a correlação entre as variáveis numéricas utilizando um gráfico de calor.
- **Gráficos de Dispersão**: Mostram a relação entre o investimento em cada plataforma (YouTube, Facebook, Newspaper) e as vendas.

### 3. Análise de Correlação
A matriz de correlação foi gerada para entender a força da relação entre as variáveis. O coeficiente de correlação indica a intensidade dessa relação, com valores próximos de 1 ou -1 indicando correlação forte.

### 4. Modelo de Regressão Linear
Foi criado um modelo de regressão linear para prever as vendas com base nos investimentos nas plataformas de marketing.

- **Divisão dos Dados**: O conjunto de dados foi dividido em treino e teste (80% treino, 20% teste).
- **Treinamento**: O modelo foi treinado utilizando a biblioteca `scikit-learn`.
- **Avaliação**: O desempenho do modelo foi avaliado com base no erro quadrático médio (MSE) e o coeficiente de determinação (R²).

## Resultados

- A análise revelou que o investimento no YouTube tem uma correlação forte e positiva com as vendas, enquanto o Facebook e o jornal apresentaram correlações mais fracas.
- O modelo de regressão linear obteve um **R²** de **0.87**, o que indica uma boa capacidade de previsão das vendas com base nos investimentos.

## Como Executar

1. Instale as dependências necessárias:
   ```bash
   pip install pandas matplotlib seaborn scikit-learn
