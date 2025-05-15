# 🕵️ Algoritmos Não Supervisionados

Os algoritmos não supervisionados são utilizados quando os dados de entrada não possuem rótulos. O principal objetivo desse algoritmo é identificar automaticamente padrões ou relacionamentos ocultos, revelando insights que poderiam passar despercebidos em uma análise tradicional.

## 🧲 Affinity Propagation

### ⚙️ Principais Características
O **Affinity Propagation** é um algoritmo de agrupamento que identifica automaticamente o número de clusters com base nas similaridades entre os dados. Ele funciona trocando mensagens entre pares de amostras, ajustando iterativamente quais pontos devem ser os representantes de cada cluster.

### ✅ Vantagens
* **Clusters Determinados Automaticamente:** Não requer que o usuário defina previamente o número de grupos.

* **Capta Estruturas Complexas:** Funciona bem com clusters de formas variadas.

* **Identifica Exemplares Representativos:** Escolhe pontos reais como representantes de cada grupo.

### ❌ Desvantagens
* **Alto Custo Computacional:** Pode ser lento para grandes volumes de dados.

* **Dependente da Similaridade:** Resultados podem variar dependendo da função de similaridade escolhida.

* **Pouco Escalável:** Não recomendado para datasets muito grandes.

### 🎯 Principais Aplicações
* **Agrupamento de Imagens e Documentos**
* **Segmentação de Dados**
* **Reconhecimento de Padrões**

<br>

## 📦 DBSCAN

### ⚙️ Principais Características
O **DBSCAN** é um algoritmo de agrupamento baseado em densidade que forma clusters a partir de regiões de alta densidade de pontos. O algoritmo define como “núcleo” um ponto que possui um número mínimo de vizinhos dentro de uma determinada distância. A partir desses núcleos, os clusters são formados por pontos densamente conectados, enquanto os pontos que não atendem aos critérios são classificados como ruído.

### ✅ Vantagens
* **Não Requer Número de Clusters:** Define os grupos com base na densidade dos dados.

* **Identificação Automática de Outliers:** Distingue naturalmente os ruídos.

* **Detecção de Clusters de Forma Arbitrária:** Consegue identificar clusters com formas complexas.

### ❌ Desvantagens
* **Sensível à escolha dos parâmetros:** A performance do algoritmo depende fortemente de uma boa escolha do *eps* e *min_samples*.

* **Desempenho Ruim em Densidade Variável:** Não lida bem com clusters com diferentes densidades.

* **Baixo Desempenho em Alta Dimensionalidade:** Em espaços de muitas dimensões, a noção de "distância" perde significado, o que reduz a eficácia do algoritmo.

### 🎯 Principais Aplicações
* **Detecção de Anomalias**
* **Análise Geoespacial**
* **Segmentação de Clientes**

<br>

## 🌳 Hierarchical Clustering

### ⚙️ Principais Características
O **Hierarchical Clustering** é um algoritmo de aprendizado que agrupa dados formando uma estrutura em árvore (dendrograma), revelando relações hierárquicas entre os elementos. Essa técnica permite identificar padrões e conexões em conjuntos de dados, sendo útil para análises exploratórias e visualização de relações entre clusters.

### ✅ Vantagens
* **Visualização com Dendrograma:** Fácil de entender a estrutura dos dados.
  
* **Não precisa definir o Número de Clusters:** O número ideal pode ser escolhido após analisar o dendrograma.

* **Detecta Subgrupos Naturais:** Útil para dados com múltiplas camadas de agrupamento.

### ❌ Desvantagens
* **Pouco Escalável:** Alto custo computacional para grandes conjuntos de dados.

* **Não se ajusta dinamicamente:** Não tem flexibilidade para corrigir junções ou divisões anteriores.

* **Sensível a Ruídos e Outliers:** Não possui mecanismos robustos para lidar com anomalias ao construir a hierarquia.

### 🎯 Principais Aplicações
* **Redução de Dimensionalidade e Pré-processamento**
* **Agrupamento de Documentos**
* **Taxonomia Biológica**

<br>

## 📍 K-Means

### ⚙️ Principais Características
O **K-Means** é um algoritmo de agrupamento que divide os dados em K grupos com base na similaridade, sendo essa similaridade geralmente medida pela distância euclidiana. Cada grupo é representado por um **Centroide**, que corresponde à média dos pontos pertencentes ao respectivo grupo. O algoritmo ajusta iterativamente os centroides até que eles se estabilizem, buscando minimizar a distância entre os pontos e seus centroides.

### ✅ Vantagens
* **Simples de Implementar:** O modelo é simples e pode ser facilmente descrito com parâmetros matemáticos.

* **Escalável para grandes conjuntos de dados:** Especialmente quando o número de *clusters* é pequeno.

* **Fácil de Interpretar:** Cada ponto é atribuído ao grupo cujo centróide está mais próximo.

* **Rápido para dados de alta dimensionalidade:** Utiliza cálculos vetoriais simples.

### ❌ Desvantagens
* **O número de *clusters* K deve ser definido previamente:** É necessário determinar o valor de K antes da execução do algoritmo, o que pode ser desafiador sem conhecimento prévio sobre a estrutura dos dados.

* **Sensível a Outliers:** Pontos muito distantes podem distorcer a posição dos centroides.

* **Pode convergir para mínimos locais:** A escolha aleatória dos centroides iniciais pode encontrar soluções que não são ideais.

### 🎯 Principais Aplicações
* **Agrupamento de Produtos**
* **Detecção de Anomalias**
* **Análise Geoespacial**

<br>

## 📉 PCA (Principal Component Analysis)

### ⚙️ Principais Características
O **PCA** é um algoritmo de **redução de dimensionalidade**. Ele transforma o conjunto de dados original em um novo sistema de coordenadas, mantendo a maior variabilidade dos dados com o menor número de variáveis possível (componentes principais).

### ✅ Vantagens
* **Redução de Ruído:** Ao eliminar componentes menos relevantes, melhora o desempenho de outros modelos.

* **Facilidade de Visualização:** Facilita a análise visual de datasets multidimensionais.

* **Melhora o Desempenho Computacional:** Reduz a dimensionalidade mantendo a maior parte da informação.

### ❌ Desvantagens
* **Perda de Interpretabilidade:** As novas variáveis (componentes principais) não têm significado direto.

* **Assume Linearidade:** Não captura bem relações não lineares.

* **Pode eliminar Informações Importantes:** Se os componentes principais não representarem bem a variabilidade dos dados.

### 🎯 Principais Aplicações
* **Pré-processamento de Dados para Machine Learning**
* **Visualização de Dados Complexos**
* **Compressão de Dados**

<br>

## 🔗 Referências

### 📚 Conceitos Gerais de Aprendizado Não Supervisionado
* [Oracle - Aprendizado Não Supervisionado](https://www.oracle.com/br/artificial-intelligence/machine-learning/unsupervised-learning/)
* [Deep Learning Book](https://www.deeplearningbook.com.br/)
* [Kaggle – Iris Dataset](https://www.kaggle.com/datasets/uciml/iris)

---

### 🧲 Affinity Propagation
* [Scikit-Learn – Affinity Propagation](https://scikit-learn.org/stable/modules/clustering.html#affinity-propagation)
* [Wikipedia – Affinity Propagation](https://en.wikipedia.org/wiki/Affinity_propagation)

---

### 📦 DBSCAN
* [Scikit-Learn – DBSCAN](https://scikit-learn.org/stable/modules/clustering.html#dbscan)
* [Medium – Entendendo DBSCAN](https://gabriellm.medium.com/entendendo-dbscan-770f680d9160)

---

### 🌳 Hierarchical Clustering
* [Scikit-Learn – Hierarchical Clustering](https://scikit-learn.org/stable/modules/clustering.html#hierarchical-clustering)
* [IBM – Hierarchical Clustering](https://www.ibm.com/think/topics/hierarchical-clustering)

---

### 📍 K-Means
* [Scikit-Learn – K-Means](https://scikit-learn.org/stable/modules/clustering.html#k-means)
* [IBM – K-Means Clustering](https://www.ibm.com/br-pt/think/topics/k-means-clustering)

---
### 📉 PCA (Principal Component Analysis)
* [Scikit-Learn – Principal Component Analysis (PCA)](https://scikit-learn.org/stable/modules/decomposition.html#principal-component-analysis-pca)
* [IBM – Principal Component Analysis](https://www.ibm.com/think/topics/principal-component-analysis)
