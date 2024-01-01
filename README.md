# arvores_tarefa3

# Reconhecimento de Atividade Humana com Árvores de Decisão

Este projeto tem como objetivo explorar a utilização de árvores de decisão para reconhecimento de atividade humana com base em dados coletados de sensores em dispositivos móveis.

## Conjuntos de Dados

Os conjuntos de dados utilizados neste projeto foram previamente processados e estão disponíveis nos arquivos `X_train_processed.csv` e `X_test_processed.csv`. Os rótulos correspondentes podem ser encontrados em `y_train.txt` e `y_test.txt`.

## Pré-processamento

O pré-processamento dos dados envolve a seleção das três melhores variáveis, conforme identificado em tarefas anteriores. Além disso, são calculados os valores de `ccp_alpha` para determinar a complexidade-custo da árvore.

## Grid Search

O Grid Search é utilizado para encontrar os melhores hiperparâmetros para o modelo de árvore de decisão. A busca é realizada em uma grade de valores de `ccp_alpha` e `max_features`. O resultado é um modelo otimizado para a tarefa de reconhecimento de atividade humana.

## Avaliação da Árvore

O melhor modelo encontrado é avaliado na base de testes, e a acurácia é calculada. Além disso, a matriz de confusão é visualizada para entender o desempenho do modelo em cada classe.

## Melhorando a Árvore

Para melhorar o desempenho do modelo, uma nova variável binária é criada para uma das classes de maior erro. Uma árvore de classificação é treinada com novas variáveis, e o processo de avaliação é repetido.

## Como Executar

Certifique-se de ter as dependências instaladas:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
