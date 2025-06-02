# ShopifyQL
## Introdução ao ShopifyQL e ao Editor de Consultas para lojas Shopify

---

### Visão Geral

O ShopifyQL (Shopify Query Language) é a linguagem de consulta desenvolvida especificamente pela Shopify para o universo de comércio eletrônico. Ele permite que você acesse e explore os dados da sua própria loja diretamente no Shopify Analytics, consultando o banco de dados e gerando relatórios detalhados e personalizados. 

Linguagens de consulta são usadas para solicitar e recuperar dados de bancos de dados. Os dados da sua loja são armazenados em tabelas de banco de dados, estruturadas em colunas e linhas definidas. As colunas definem o tipo de informação que contêm, como vendas, e as linhas especificam o valor real do tipo de dado.

Com o editor de consultas ShopifyQL, você consegue visualizar informações aprofundadas sobre o desempenho da sua loja, personalizar suas análises e gerar relatórios sob medida, sem depender apenas dos relatórios padrão **e é aqui que entra o ShopifyQL**.

Para quem utiliza Shopify de forma profissional, reconhecemos o impacto positivo que decisões orientadas por dados têm no crescimento de um negócio. Mas também sabemos que a exploração de dados costuma ser inacessível para quem não possui formação em ciência de dados ou programação. O ShopifyQL e o editor de relatórios (acessível em Análises > Relatórios > Nova Exploração) tornou mais fácil o uso de dados na tomada de decisões para os lojistas ao criar uma linguagem de consulta acessível e focada em lojas Shopify: ShopifyQL.

O ShopifyQL permite que lojistas da Shopify de todos os planos explorem seus dados com recursos avançados como:

- Sintaxe simples e fácil de aprender.
- Visualização de dados integrada em um único passo.
- Comparações automáticas de períodos.
- Funções de data específicas para o comércio.

Aqui, vou abordar como o ShopifyQL torna a exploração de dados mais acessível, apresentaremos os recursos específicos para o comércio que incorporamos à linguagem e faremos uma demonstração com alguns exemplos de queries.

### Onde usar?

Você pode usar o ShopifyQL com o novo Shopify Analytics para explorar o banco de dados da sua própria loja e recuperar os dados que oferecem uma compreensão mais aprofundada do seu negócio. Para recuperar seus dados em um formato significativo, uma consulta deve ser enviada ao banco de dados. Uma consulta é uma Query que solicita dados específicos como resposta, composta por palavras-chave e seus parâmetros correspondentes. A combinação de várias palavras-chave com parâmetros específicos constrói sua consulta. Após montar sua consulta, você pode executá-la e receber um relatório.

---

### O que é o ShopifyQL?

ShopifyQL é uma linguagem de consulta otimizada para o contexto do uso dos dados de relatórios por uma loja Shopify. Assim como outras linguagens de consulta (como SQL), ela permite solicitar e recuperar dados armazenados em um banco de dados.

No caso da Shopify, os dados da sua loja estão armazenados em tabelas de banco de dados que possuem estrutruas básicas como:

**Colunas**: definem o tipo de informação (ex.: sales, orders, customers).
**Linhas**: contêm os valores reais (ex.: USD 2,450 em vendas).

---

### Como funciona uma consulta no ShopifyQL?

Para obter dados no formato desejado, você precisa construir uma consulta (query).
Uma consulta é, essencialmente, uma pergunta que você faz ao banco de dados, formada por:

- **Palavras-chave (keywords)**: são as instruções base da consulta.
- **Parâmetros**: são os filtros e definições específicas.

Exemplo simplificado de estrutura de query:

<code>FROM sales
  SHOW total_sales, customers
  WHERE day >= '2025-01-01' AND day <= '2025-06-02'
  GROUP BY month</code>
