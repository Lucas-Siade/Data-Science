# 💡 Algoritmos Supervisionados

Os algoritmos supervisionados utilizam conjuntos de dados rotulados para treinar modelos que fazem previsões ou classificações com base em exemplos anteriores. Esse tipo de algoritmo utiliza os valores passados da variável alvo para aprender quais devem ser seus resultados de saída, ajustando-se até que o erro tenha sido suficientemente minimizado.

## 📏 Regressão Linear

### ⚙️ Principais Características
A Regressão Linear é um algoritmo que busca encontrar uma reta que melhor se ajusta aos dados, descrevendo a relação entre uma ou mais variáveis independentes e uma variável dependente. A Regressão Linear é amplamente aplicada em problemas de previsão de valores contínuos, onde o objetivo é estimar o resultado de uma variável com base em valores conhecidos das outras variáveis.

### ✅ Vantagens
* **Fácil de Implementar e Interpretar:** O modelo é simples de entender e pode ser facilmente descrito com parâmetros matemáticos.

* **Pouco Custo Computacional:** O treinamento é rápido e ideal para conjuntos de dados pequenos e médios.

* **Coeficientes Interpretáveis:** Os pesos indicam claramente o impacto de cada variável, o que facilita análises de negócio e decisões.

### ❌ Desvantagens
* **Limitação com Relações Não Lineares:** Se a relação entre as variáveis for curva, circular ou qualquer padrão não-reto, a Regressão Linear não conseguirá representar bem.

* **Vulnerável a Outliers:** Valores extremos podem distorcer muito o modelo final, gerando previsões erradas.

* **Não é ideal para Classificação:** Mesmo que seja possível, a Regressão Linear não é recomendável para classificar.

### 🎯 Principais Aplicações
* **Previsão de Valores**
* **Estimatica de Preços**
* **Projeção de Lucros e Despesas**
* **Análise de Tendências**

<br>

## 🔢 Regressão Logística

### ⚙️ Principais Características
A Regressão Logística, apesar do nome, é um modelo utilizado para Classificação, e não para Regressão. Ela prevê a probabilidade de um exemplo pertencer a uma determinada classe, geralmente em problemas de classificação binária. Sua principal característica é a função sigmoide, que transforma a saída em um valor entre 0 e 1, tornando possível a interpretação como uma probabilidade.

### ✅ Vantagens
* **Eficiência computacional:** Requer menos poder computacional em comparação com redes neurais ou algoritmos mais complexos.

* **Generalização:** Funciona bem quando há uma relação linear entre as variáveis independentes e a probabilidade do evento.

* **Probabilidades de saída:** Fornece a probabilidade de pertencimento a uma classe.

### ❌ Desvantagens
* **Não funciona bem com dados não lineares:** Se os dados não forem linearmente separáveis, o modelo terá um desempenho insatisfatório.

* **Sensível a Outliers:** Outliers podem impactar os coeficientes e reduzir a precisão do modelo.

* **Requer melhor preparação dos dados:** Pode exigir transformações e normalizações para melhor desempenho.

### 🎯 Principais Aplicações
* **Detecção de Fraudes**
* **Diagnóstico de Doenças**
* **Análise de Clientes**

<br>

## 📍 K-Nearest Neighbor (KNN)

### ⚙️ Principais Características
O **K-Nearest Neighbor (KNN)** é um algoritmo não paramétrico, ou seja, não tenta ajustar alguma função matemática aos dados. Suas previsões são baseadas na distância entre os pontos do conjunto de dados, atribuindo o resultado com base nos K exemplos mais próximos da amostra de teste.  O algoritmo pode ser aplicado tanto para **Regressão** quanto para **Classificação**, embora seja mais comumente utilizado em tarefas de classificação.

### ✅ Vantagens
* **Fácil de Implementar:** É um algoritmo intuitivo, com poucos parâmetros e simples de entender.

* **Dispensa Fase de Treinamento:** Armazena diretamente os dados de treino, o que reduz o tempo de preparação.

* **Lida bem com Múltiplas Classes:** Apresenta bom desempenho em problemas de classificação com mais de duas categorias.

* **Eficiente com Dados bem separados:** Funciona muito bem quando as classes estão nitidamente separadas.

### ❌ Desvantagens
* **Alto Custo Computacional:** Exige o cálculo da distância entre a amostra de teste e todos os pontos do conjunto de treino.

* **Sensível a Ruídos e Outliers:** Dados fora do padrão podem distorcer as previsões e afetar negativamente a acurácia.

* **Escolha do K Ideal é crucial** Valores muito pequenos ou muito altos de K podem prejudicar o desempenho.

### 🎯 Principais Aplicações
* **Detecção de Anomalias**
* **Recomendação de Produtos**
* **Classificação de Doenças**
* **Reconhecimento de Imagens**

<br>

## 🌲 Random Forest

### ⚙️ Principais Características
A **Random Forest** é um algoritmo de aprendizado baseado em um conjunto de árvores de decisão. Ele utiliza a técnica de Bagging (Bootstrap Aggregating) para criar múltiplos subconjuntos aleatórios dos dados de treinamento. Cada uma dessas árvores é treinada com uma amostra diferente dos dados, selecionando aleatoriamente um subconjunto de variáveis.

### ✅ Vantagens
* **Alta Precisão:** A combinação de subconjuntos diferentes de dados desenvolve um modelo mais estável.

* **Seguro contra Overfitting:** O modelo reduz o risco de Overfitting por utilizar múltiplas árvores e fazer uma "votação" dos resultados.

* **Lida com dados faltantes:** O modelo pode estimar os valores ausentes utilizando a média ponderada das observações ou utilizar árvores de decisão para preencher lacunas.

* **Indica a importância das variáveis usadas na predição:** Consegue avaliar o impacto de cada variável e atribuir um peso de importância.

### ❌ Desvantagens
* **Dificuldade de interpretar os resultados:** A decisão final vem da junção de muitas árvores.

* **Consome mais memória:** O modelo precisa armazenar múltiplas árvores de decisão.

* **Não funciona bem com dados lineares:** Para problemas lineares, o modelo pode ser um exagero e até gerar previsões menos eficientes.

### 🎯 Principais Aplicações
* **Relações Bancárias**
* **Diagnóstico Médico**
* **Previsão no Mercado Financeiro**

<br>

## ⚡ Support Vector Machine (SVM)

### ⚙️ Principais Características
O **Support Vector Machine** é um algoritmo que pode ser aplicado tanto para **Regressão** quanto para **Classificação**. O seu principal objetivo é encontrar o melhor hiperplano que separa os dados, maximizando a distância entre os grupos diferentes em um espaço N-dimensional.

### ✅ Vantagens
* **Eficiente em espaços de alta dimensionalidade:** O SVM mantém bom desempenho mesmo quando o conjunto de dados possui diversas *features*.

* **Eficiente com poucos dados:** O SVM foca apenas no pontos mais relevantes - chamados de **vetores de suporte** - para definir a fronteira de decisão.

* **Versátil:** Diferentes funções de Kernel podem ser aplicadas de acordo com o problema, permitindo que se adapte tanto a dados linearmente separáveis quanto a relações complexas.

### ❌ Desvantagens
* **Não é tão escalável:** O treinamento do modelo se torna cada vez mais difícil à medida que o número de amostras aumenta.

* **Sensível à escolha do Kernel:** Uma configuração inadequada do Kernel pode comprometer a capacidade de generalização do modelo.

* **Difícil de interpretar Kernels não lineares:** Quando utiliza funções complexas, como RBF ou Polinomial, o modelo se torna mais difícil de interpretar e entender como as decisões são tomadas.

* **Não fornece probabilidade:** Por padrão, o modelo não calcula a probabilidade das previsões apenas realiza uma classificação direta.

### 🎯 Principais Aplicações
* **Classificação de Texto**
* **Bioinformática**
* **Classificação de Imagens**

🔗 Referências
