# Case 5

#### No banco de dados da Dadosfera, temos uma tabela chamada "users_email" contendo detalhes do usuário. Escreva uma consulta SQL que seleciona usuário que se cadastraram nos último 30 dias e envie um relatório com esses dados. Por favor, explique o que cada parte da consulta faz.

```
SELECT \*FROM users_emailWHERE data_cadastro >= DATE_SUB(CURDATE( ), INTERVAL 30 DAY);
```

###### Nesse comando estou selecionando tudo da tabela users_email, então adiciono uma espécie de condição, filtro, ONDE ele vai me retornar apenas aqueles em que a data_cadastro seja maior ou igual à data atual (CURDATE) menos 30 dias (INTERVAL 30 DAY).

###### Ex.:

```
SELECT \*FROM users_emailWHERE data_cadastro >= DATE_SUB(08-03-2023, INTERVAL 30 DAY);
```
