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

## 📊 Gaussian Mixture Model

### ⚙️ Principais Características
O **Gaussian Mixture Model** é um algoritmo de agrupamento baseado em modelos probabilísticos. Ele modela a distribuição dos pontos como uma combinação de múltiplas distribuições gaussianas, onde cada uma representa um possível grupo, e calcula a probabilidade de cada ponto pertencer a cada grupo.

### ✅ Vantagens
* **Atribuição Suave:** Em vez de designar cada ponto a um único cluster, fornece a probabilidade de pertencimento a todos os clusters.
  
* **Capta Estruturas Complexas:** Capaz de identificar clusters com diferentes formas, tamanhos e orientações.

* **Base Estatística Robusta:** Permite análise mais rica e interpretável com base em distribuições gaussianas.

### ❌ Desvantagens
* **O número de *clusters* deve ser definido previamente:** Requer a escolha prévia do número de componentes (clusters).

* **Sensível a Outliers:** Pode ser afetado por pontos fora do padrão, pois tenta ajustar gaussianas a todos os dados.

* **Mais Complexo Computacionalmente:** Envolve muitos cálculos de probabilidades e estimação de parâmetros.

### 🎯 Principais Aplicações
* **Reconhecimento de Padrões**
* **Reconhecimento de Fala**
* **Análise de Clientes**

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

## 🌀 Kernel PCA (Principal Component Analysis com Núcleo)

### ⚙️ Principais Características
O **Kernel PCA** é uma extensão não linear do PCA tradicional que utiliza funções kernel para mapear os dados originais para um espaço de alta dimensão, onde é possível realizar a análise de componentes principais de forma linear. Isso permite capturar estruturas não lineares dos dados que o PCA clássico não consegue detectar.

### ✅ Vantagens
* **Capta Relações Não Lineares:** Permite identificar componentes principais em dados com estrutura não linear.
  
* **Flexível:** Pode usar diferentes tipos de kernels (RBF, polinomial, sigmoidal, etc.) para adaptar-se ao formato dos dados.

* **Melhora a Redução de Dimensionalidade:** Pode melhorar a representação dos dados em espaços menores mantendo a estrutura relevante.

### ❌ Desvantagens
* **Mais Complexo Computacionalmente:** Para grandes conjuntos de dados, o cálculo da matriz kernel pode ser caro em tempo e memória.

* **Sensível à Escolha do Kernel:** O desempenho depende fortemente da escolha do kernel e seus parâmetros.

* **Menos Interpretável:** Os componentes principais resultantes em espaços kernel são menos intuitivos do que no PCA clássico.

### 🎯 Principais Aplicações
* **Reconhecimento de Padrões Não Lineares**
* **Redução de Dimensionalidade para Dados Complexos**
* **Pré-processamento de Dados para Machine Learning**

<br>

## 🗺️ t-SNE (t-Distributed Stochastic Neighbor Embedding)

### ⚙️ Principais Características
O **t-SNE** é um algoritmo de redução de dimensionalidade não linear, especialmente eficaz para visualização de dados em 2D ou 3D. Ele transforma as distâncias entre pontos em probabilidades de similaridade e busca preservar as relações locais.

### ✅ Vantagens
* **Bom para Visualização:** É eficaz para representar dados complexos em duas ou três dimensões.

* **Captura Relações Locais:** Mantém a proximidade entre os pontos similares, revelando padrões e agrupamentos.

* **Revela Estrutura dos Dados:** Muitas vezes revela clusters que não seriam evidentes com métodos lineares.

### ❌ Desvantagens
* **Não Escalável para Grandes Conjuntos de Dados:** A complexidade computacional cresce rapidamente com o tamanho dos dados.

* **Sensível a Parâmetros:** O resultado depende da escolha certa de parâmetros como *perplexity* e *learning rate*.

* **Não é Determinístico:** Execuções repetidas podem gerar resultados diferentes.

### 🎯 Principais Aplicações
* **Visualização de Dados de Alta Dimensionalidade**
* **Análise Exploratória de Agrupamentos**
* **Redução de Dimensionalidade para Dados de Imagem**

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

### 📊 Gaussian Mixture Model
* [Scikit-Learn – Gaussian Mixture](https://scikit-learn.org/stable/modules/mixture.html#gaussian-mixture)
* [Built In – Gaussian Mixture Model](https://builtin.com/articles/gaussian-mixture-model)

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

---

### 🌀 Kernel PCA (Principal Component Analysis com Núcleo)
* [Scikit-Learn – Kernel Principal Component Analysis (KPCA)](https://scikit-learn.org/stable/modules/decomposition.html#kernel-principal-component-analysis-kpca)
* [Baeldung – Kernel Principal Component Analysis (KPCA)](https://www.baeldung.com/cs/kernel-principal-component-analysis)  

---

### 🗺️ t-SNE (t-Distributed Stochastic Neighbor Embedding)
* [Scikit-Learn – t-Distributed Stochastic Neighbor Embedding (t-SNE)](https://scikit-learn.org/stable/modules/manifold.html#t-distributed-stochastic-neighbor-embedding-t-sne)  
* [DataCamp – Introdução ao t-SNE](https://www.datacamp.com/pt/tutorial/introduction-t-sne)  
* [Wikipedia – t-distributed Stochastic Neighbor Embedding](https://en.wikipedia.org/wiki/T-distributed_stochastic_neighbor_embedding)
