# Análise de Dados de Empregabilidade

## Objetivo do Projeto
Este projeto tem como objetivo analisar o desempenho acadêmico e experiência profissional de candidatos com base em um dataset de colocação profissional. O foco é explorar as relações entre diferentes atributos e o status de empregabilidade, além de criar um modelo preditivo para determinar a probabilidade de um candidato ser colocado.

## Descrição do Dataset
O dataset utilizado possui informações detalhadas sobre histórico educacional e experiência de trabalho dos candidatos. Os atributos estão descritos a seguir:

- **gender**: Gênero do candidato.
- **ssc_percentage**: Percentual de notas nos exames do ensino fundamental (10ª série).
- **ssc_board**: Conselho educacional responsável pelos exames do ensino fundamental.
- **hsc_percentage**: Percentual de notas nos exames do ensino médio (12ª série).
- **hsc_board**: Conselho educacional responsável pelos exames do ensino médio.
- **hsc_subject**: Área de estudo no ensino médio.
- **degree_percentage**: Percentual de notas na graduação.
- **undergrad_degree**: Área de estudo na graduação.
- **work_experience**: Experiência profissional anterior.
- **emp_test_percentage**: Percentual obtido em um teste de aptidão.
- **specialization**: Especialização no MBA (majors).
- **mba_percent**: Percentual de notas no MBA.
- **status**: Status de colocação profissional (Target). Valores: *Placed* ou *Not Placed*.

## Etapas do Projeto

### 1. Carregamento e Visualização dos Dados
- Carregamento do dataset `Job_Placement_Data.csv`.
- Apresentação inicial dos dados com as primeiras linhas do dataframe.
- Verificação de valores ausentes e tratamento, quando necessário.

### 2. Análise Exploratória de Dados (EDA)
- Distribuição das notas por diferentes exames (ensino fundamental, médio, graduação, MBA).
- Análise de relação entre as variáveis e o status de empregabilidade.
- Geração de:
  - Histogramas para distribuições.
  - Boxplots para identificar outliers.
  - Matriz de correlação visualizada com `heatmap`.

### 3. Modelagem Supervisionada
- Utilização do modelo **AdaBoostClassifier**.
- Divisão dos dados em conjunto de treino e teste.
- Avaliação do modelo com:
  - Acurácia.
  - Relatório de classificação (precision, recall, f1-score).

### 4. Resultados e Conclusões
- Identifica os atributos mais relevantes para a predição do status de empregabilidade.
- O modelo **AdaBoostClassifier** apresentou [inserir métrica de acurácia do modelo aqui] de acurácia.
- Observa-se que atributos como **mba_percent**, **degree_percentage** e **emp_test_percentage** tiveram maior impacto no status de colocação.


## Limitações
- Este projeto foca apenas em modelos supervisionados. Uma abordagem não supervisionada (clusterização) será explorada em futuros trabalhos.

## Tecnologias e Ferramentas
- Linguagem: Python
- Bibliotecas principais:
  - pandas
  - numpy
  - matplotlib
  - seaborn
  - scikit-learn

## Como Executar
1. Clone o repositório contendo este projeto.
2. Certifique-se de ter todas as dependências instaladas:
   ```bash
   pip install 
   ```
3. Execute o notebook `analise1.ipynb` para reproduzir a análise.
