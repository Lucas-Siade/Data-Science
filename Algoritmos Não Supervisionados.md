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
O DBSCAN é um algoritmo de agrupamento baseado em densidade que forma clusters a partir de regiões de alta densidade de pontos. O algoritmo define como “núcleo” um ponto que possui um número mínimo de vizinhos dentro de uma determinada distância. A partir desses núcleos, os clusters são formados por pontos densamente conectados, enquanto os pontos que não atendem aos critérios são classificados como ruído.

### ✅ Vantagens
* **Não Requer Número de Clusters:** Define os grupos com base na densidade dos dados.

* **Identificação Automática de Outliers:** Distingue naturalmente os ruídos.

* **Detecção de Clusters de Forma Arbitrária:** Consegue identificar clusters com formas complexas

### ❌ Desvantagens
* **Sensível à escolha dos parâmetros:** A performance do algoritmo depende fortemente de uma boa escolha do *eps* e *min_samples*.

* **Desempenho Ruim em Densidade Variável:** Não lida bem com clusters com diferentes densidades.

* **Baixo Desempenho em Alta Dimensionalidade:** Em espaços de muitas dimensões, a noção de "distância" perde significado, o que reduz a eficácia do algoritmo.

### 🎯 Principais Aplicações
* **Detecção de Anomalias**
* **Análise Geoespacial**
* **Segmentação de Clientes**




## 🔗 Referências

### 📚 Conceitos Gerais de Aprendizado Não Supervisionado
* [Oracle - Aprendizado Não Supervisionado](https://www.oracle.com/br/artificial-intelligence/machine-learning/unsupervised-learning/)
* [Deep Learning Book](https://www.deeplearningbook.com.br/)

---

### 🧲 Affinity Propagation

* [Scikit-Learn – Affinity Propagation](https://scikit-learn.org/stable/modules/clustering.html#affinity-propagation)
* [Wikipedia – Affinity Propagation](https://en.wikipedia.org/wiki/Affinity_propagation)

---

### 📦 DBSCAN

* [Scikit-Learn – DBSCAN](https://scikit-learn.org/stable/modules/clustering.html#dbscan)
* [Medium – Entendendo DBSCAN](https://gabriellm.medium.com/entendendo-dbscan-770f680d9160)
