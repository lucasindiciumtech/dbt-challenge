``` pip install -r requirements.txt && cd dbt && dbt seed```

# Desafio 1: Data Mart de Desempenho de Vendas
## Objetivo:
Construir um data mart que forneça uma visão agregada do desempenho de vendas por produto e categoria, incluindo métricas como receita total, quantidade vendida, e preço médio de venda.

## Modelo de Dados:
Tabelas Fonte: orders, order_items, products.
Transformações:
Filtrar apenas orders com status "Shipped".
Realizar um join entre order_items e orders para garantir que apenas itens de pedidos enviados sejam considerados.
Agregar dados ao nível de produto, somando a quantidade vendida e a receita total.
Calcular o preço médio de venda por produto.



# Desafio 2: Data Mart de Comportamento do Cliente
## Objetivo:
Desenvolver um data mart que segmente os clientes com base no valor total de compras e na frequência de compras, identificando clientes VIPs, regulares e esporádicos.

# Modelo de Dados:
Tabelas Fonte: customers, orders.
Transformações:
Filtrar orders com status "Shipped".
Agregar dados ao nível de cliente, calculando o valor total de compras e o número total de pedidos.
Segmentar clientes com base em critérios pré-definidos (por exemplo, VIPs: >$500 em compras e mais de 5 pedidos).