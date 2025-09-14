# Exercício IA / Etapa 1 - Bruno de Medeiros e José Kayky -  

## Perguntas: 
### 1. O que significa classificação supervisionada?
É um tipo de aprendizado de máquina, onde o modelo aprende a partir de um conjunto de dados rotulado, por exemplo, o dataset de transações PIX, cada registro está marcado como “fraude” ou “não fraude”, dessa forma modelo aprende com essas informações e depois pode prever se uma nova transação é fraudulenta ou não.

### 2. Qual é a importância de dividir o dataset em conjunto de treino e teste?
Garantir a avaliação real de desempenho do modelo em dados inéditos, dividindo em teste e treino, garante que o modelo seja capaz de generalizar e evita a falha em novos dados.

### 3. Qual a diferença entre Decision Tree e KNN em termos de funcionamento?
O Decision Tree cria uma estrutura em forma de árvore, onde cada nó representa uma pergunta sobre uma feature, sendo facilmente entendível o caminho que levou a decisão.

O KNN não constrói um modelo explícito, ele apenas compara um novo ponto com os vizinhos mais próximos na feature e a classe é decidida pela maioria dos vizinhos.

# Sobre o Dataset:
O Dataset contém 10.000 registros sintéticos de recebimentos de transações PIX, incluindo anomalias inseridas artificialmente (1%) para simulação e treinamento de modelos antifraude.

O principal objetivo é fornecer um banco de dados para estudos em:

Detecção de fraude financeira em tempo real;

Análise de anomalias em sistemas de pagamento;

Construindo aprendizado de máquina e modelos de aprendizado profundo aplicados a transações bancárias;

A inspiração vem do crescente número de transações digitais no Brasil e da necessidade de desenvolver soluções inteligentes de prevenção de fraudes.

## Resultados da Análise:
**DECISION TREE**
```
Acurácia: 0.9845
F1-Score: 0.3673
Matriz de Confusão:
[[1960   13]
[  18    9]]
```

**KNN**
```
Acurácia: 0.9895
F1-Score: 0.3636
Matriz de Confusão:
[[1973    0]
[  21    6]]
```
**LOGISTIC REGRESSION**
```
Acurácia: 0.9880
F1-Score: 0.2000
Matriz de Confusão:
[[1973    0]
[  24    3]]
```

## Conclusão:
Por ser um dataset onde os dados de fraude representavam a minoria, ou seja, de 10000 resultados, apenas 100 eram fraudes,  a comparação dos 3 modelos resultou uma acurácia muito alta e parecida. Dessa forma, o modelo KNN mostrou uma melhor solução.

Como a base tem 1% de dados fraudulentos, isto é, poucos exemplos para o treinamento da inteligência artificial. Logo, espera-se um resultado muito alto.
