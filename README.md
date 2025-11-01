# analise-cluster-clientes-shopping
## O Problema de Negócio

Um shopping center deseja otimizar suas estratégias de marketing, mas atualmente utiliza uma comunicação genérica para todos os seus clientes. A falta de direcionamento resulta em baixo engajamento e desperdício de recursos.

A pergunta central é: **Como podemos agrupar nossos clientes em segmentos distintos com base em seu comportamento e demografia para criar campanhas de marketing mais eficazes e personalizadas?**

## Tecnologias Utilizadas

* **Python:** Linguagem principal da análise.
* **Pandas:** Para manipulação e tratamento dos dados.
* **Scikit-learn (`sklearn`):** Para aplicação do modelo de clusterização K-Means.
* **Seaborn & Matplotlib:** Para visualização e interpretação dos clusters.
* **Jupyter Notebook:** Como ambiente de desenvolvimento e storytelling.

## Metodologia

O projeto seguiu uma metodologia clara de análise de dados:

1.  **Coleta e Preparação:** Os dados de clientes do shopping foram carregados e inspecionados. Foi realizado um tratamento para verificar valores nulos e garantir a integridade dos dados.
2.  **Seleção de Features:** Com base no problema de negócio, foram selecionadas as colunas mais relevantes para o modelo: `Idade`, `Renda Anual` e `Poder de Compra (Spending Score)`.
3.  **Modelagem K-Means:** Foi aplicado o modelo `KMeans` da biblioteca `scikit-learn`, definindo **5 clusters** (grupos) como o número ideal para uma segmentação acionável.
4.  **Visualização e Interpretação:** Os clusters resultantes foram plotados e analisados para identificar as "personas" de cada grupo.

## Resultados: As 5 Personas de Clientes

A análise revelou 5 grupos de clientes distintos e bem definidos, visualizados claramente na relação entre Renda e Poder de Compra:

<img width="847" height="741" alt="image" src="https://github.com/user-attachments/assets/f1929e44-3603-4079-a182-b4990aea2e4d" />


### Interpretação dos Clusters:

* #### Cluster 0 (Azul): O Cliente Ideal (Alvo)
    * **Perfil:** Renda ALTA e Poder de Compra ALTO.
    * **Análise:** É o grupo mais valioso. Têm dinheiro e gostam de gastar.

* #### Cluster 1 (Laranja): O Poupador Rico (Cauteloso)
    * **Perfil:** Renda ALTA, mas Poder de Compra BAIXO.
    * **Análise:** Clientes com potencial, mas que são cautelosos com gastos. Precisam de estratégias focadas em valor e qualidade.

* #### Cluster 2 (Verde): O Consumidor Padrão (Equilibrado)
    * **Perfil:** Renda MÉDIA e Poder de Compra MÉDIO.
    * **Análise:** Representa o cliente "médio" do shopping, com gastos proporcionais à sua renda.

* #### Cluster 3 (Vermelho): O Jovem Gastador (Impulsivo)
    * **Perfil:** Renda BAIXA, mas Poder de Compra ALTO. São notavelmente mais jovens.
    * **Análise:** Provavelmente jovens que gastam a maior parte de sua renda disponível em tendências e fast-fashion.

* #### Cluster 4 (Roxo): O Econômico (Sensível a Preço)
    * **Perfil:** Renda BAIXA/MÉDIA e Poder de Compra BAIXO. Tendem a ser mais velhos.
    * **Análise:** Focados no essencial e muito sensíveis a preços. Buscam promoções e liquidações.

## Conclusões e Ações Estratégicas

A segmentação foi bem-sucedida e permitiu a criação de estratégias de marketing direcionadas, saindo do modelo genérico:

1.  **"Cliente Ideal" (Cluster 0):** Programas VIP, acesso antecipado a coleções, marketing de exclusividade.
2.  **"Poupador Rico" (Cluster 1):** Comunicação focada em qualidade, durabilidade e valor (ex: relógios, joias, artigos de luxo).
3.  **"Consumidor Padrão" (Cluster 2):** Campanhas sazonais, promoções de "custo-benefício" e programas de pontos.
4.  **"Jovem Gastador" (Cluster 3):** Marketing de influência, eventos em redes sociais, foco em tendências e fast-fashion.
5.  **"Econômico" (Cluster 4):** Clube de descontos, e-mail marketing com foco em liquidações e ofertas.

Este projeto demonstra a capacidade de transformar dados brutos em insights de negócio acionáveis através do uso de Machine Learning.
