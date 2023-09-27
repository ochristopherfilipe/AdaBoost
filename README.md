# AdaBoost vs Random Forest:

O RandomForest e o AdaBoost são dois algoritmos populares de aprendizado de máquina que pertencem à categoria de ensemble learning, onde múltiplos modelos são combinados para melhorar o desempenho de predição. Aqui estão cinco diferenças importantes entre esses dois algoritmos:

1. O AdaBoost é mais sensível a outliers, já que as amostras classificadas incorretamente recebem mais peso.
2. O Adaboost usa árvores de profundidade máxima de 1 e o maximo de 2 folhas.
3. No AdaBoost, as amostras são ponderadas de forma adaptativa durante o treinamento. No RandomForest, todas as amostras de treinamento têm o mesmo peso em cada árvore.
4. O AdaBoost se baseia na construção de pequenas árvores de decisão(Stump), que são treinadas para corrigir os erros dos modelos anteriores. O RandomForest constrói um conjunto de árvores de decisão independentes.
5. No AdaBoost, para cada iteração sucessiva, os pesos amostrais são modificados individualmente e o algoritmo de aprendizagem é reaplicado aos dados reponderados


# Os hiperparâmetros mais comuns usados com o algoritmo AdaBoost incluem:

**n_estimators**: Este hiperparâmetro controla o número de estimadores fracos (por exemplo, árvores de decisão rasas) usados no conjunto. Um valor maior geralmente leva a um desempenho melhor, mas também aumenta o tempo de treinamento.

**learning_rate**: O learning_rate determina a taxa de aprendizado do modelo. Ele controla a contribuição de cada estimador fraco para a previsão final. Um valor menor torna o modelo mais robusto, mas pode exigir um número maior de estimadores.

**estimator**: Este hiperparâmetro permite especificar o tipo de estimador fraco a ser usado. O valor padrão é geralmente uma árvore de decisão com pouca profundidade, mas você pode fornecer outros estimadores, como regressores lineares ou outros classificadores.

**algorithm**: O hiperparâmetro algorithm permite escolher o algoritmo de boosting a ser usado. Existem duas opções comuns: 'SAMME' e 'SAMME.R'. 'SAMME' é usado para classificação binária, enquanto 'SAMME.R' é usado para classificação multiclasse. 'SAMME.R' geralmente é mais robusto e convergente.

**random_state**: O random_state é usado para controlar a semente aleatória usada pelo AdaBoost. Isso torna os resultados reproduzíveis e ajuda na comparação de diferentes configurações de hiperparâmetros.
