# Análise de Clusterização e Padrões de Comportamento dos Clientes

## Objetivo

Esta análise tem como objetivo segmentar os clientes com base no comportamento de compra, utilizando técnicas de clusterização. O processo envolve a análise de recência, frequência e valor monetário das compras dos clientes, com o intuito de identificar padrões e fornecer insights para otimizar campanhas de marketing e aumentar a fidelização.

---

## Etapas Realizadas

### 1. Pré-processamento dos Dados
- **Normalização dos Dados**: Os dados foram normalizados utilizando a técnica de *StandardScaler*, garantindo que todas as variáveis estivessem em uma escala comparável.
- **Seleção das Variáveis**: Focamos nas variáveis *recência*, *frequência* e *monetário*, que são as mais relevantes para a análise de clusterização.
- **Tratamento de Dados**:
    - Remoção de **dados nulos** e **duplicados**.
    - **Identificação e remoção de outliers** utilizando a técnica de **IQR**.

### 2. Escolha do Algoritmo de Clusterização
- **Algoritmo Utilizado**: Foi escolhido o algoritmo *KMeans* para a clusterização dos dados, devido à sua eficiência e simplicidade em segmentar os dados em grupos distintos.
- **Determinação do Número de Clusters**: O número ideal de clusters foi determinado utilizando os métodos de **Elbow** e **Silhouette Score**, resultando em 2 clusters.

### 3. Análise dos Clusters Obtidos
- **Distribuição dos Clusters**: A maior parte dos clientes foi alocada no **Cluster 0**, enquanto o **Cluster 1** representou uma pequena parcela dos dados.
- **Características dos Clusters**:
    - **Cluster 0**: Representa os clientes mais frequentes, com um comportamento de compra mais regular e um valor monetário médio mais alto.
    - **Cluster 1**: Contém clientes com uma recência maior (clientes mais recentes), porém com menor frequência de compras e menor valor monetário.

### 4. Padrões Identificados
- **Cluster 0**: Clientes com maior lealdade e frequência de compra. Estratégias de **fidelização** são recomendadas.
- **Cluster 1**: Clientes mais novos, com menor frequência e valor de compra. Estratégias de **reengajamento** e **aumento de frequência** são necessárias.

---

## Insights

### 1. Diferenças Significativas entre os Clusters
- O **Cluster 0** contém a maioria dos clientes, com um comportamento de compra estável, enquanto o **Cluster 1** é composto por clientes com comportamento de compra mais esporádico.

### 2. Distribuição entre os Países
- A distribuição entre os países é **uniforme**, com a maioria dos clientes concentrada no **Cluster 0**. Isso indica que as campanhas de marketing podem ser adaptadas para esse grupo maior, visando **fidelização**.

### 3. Frequência e Valor Monetário
- **Cluster 1** apresenta uma **menor frequência** e **menor valor monetário**, indicando a necessidade de estratégias de **incentivo ao retorno** e **promoções para aumentar o valor gasto** por compra.

### 4. Padrões de Comportamento por Cluster
- **Cluster 0**: Clientes mais frequentes, com valores mais altos de compra, indicam que esse grupo é mais leal.
- **Cluster 1**: Clientes mais recentes, com menor frequência e menor valor monetário. Estratégias para **aumentar a frequência de compras** e **ticket médio** seriam vantajosas.

---

## Ações Recomendadas

- **Para Cluster 0**: Focar em campanhas de **fidelização** e **descontos exclusivos** para manter os clientes engajados.
- **Para Cluster 1**: Utilizar **promoções de retorno**, **cupons de desconto** e **estratégias para aumentar a frequência de compras**.
- **Segmentação Regional**: Considerar as peculiaridades dos diferentes **países** para campanhas mais direcionadas e específicas.

---

## Conclusão

A segmentação dos clientes por meio da clusterização permite uma abordagem mais **personalizada** nas campanhas de marketing, ajudando a otimizar os esforços e melhorar o **engajamento** e **fidelização** dos clientes. O próximo passo seria implementar as estratégias recomendadas para cada cluster e acompanhar os resultados ao longo do tempo.
