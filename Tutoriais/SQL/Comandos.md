## Banco de Dados:
- CREATE DATABASE: Cria um novo banco de dados.
- DROP DATABASE: Exclui um banco de dados existente.

## Tabela:
- CREATE TABLE: Cria uma nova tabela no banco de dados.
- ALTER TABLE: Modifica a estrutura de uma tabela existente.
- DROP TABLE: Exclui uma tabela existente.
- TRUNCATE TABLE: Remove todos os registros de uma tabela mantendo sua estrutura.

## Tipos de Dados:
- INT / INTEGER: Números inteiros.
- FLOAT: Números de ponto flutuante com precisão simples.
- DOUBLE / REAL: Números de ponto flutuante com precisão dupla.
- DECIMAL / NUMERIC: Números decimais com precisão fixa.
- CHAR: Cadeia de caracteres de tamanho fixo.
- VARCHAR: Cadeia de caracteres de tamanho variável.
- TEXT: Cadeia de caracteres de tamanho variável (maior capacidade que o VARCHAR).
- DATE: Data no formato AAAA-MM-DD.
- TIME: Horário no formato HH:MM:SS.
- DATETIME / TIMESTAMP: Data e hora no formato AAAA-MM-DD HH:MM:SS.
- BOOLEAN / BOOL: Valor lógico (verdadeiro ou falso).

## Restrição:
- ADD CONSTRAINT: Adiciona uma restrição a uma tabela existente.
- DROP CONSTRAINT: Remove uma restrição existente em uma tabela.
- CHECK: Define uma restrição para verificar se os valores em uma coluna atendem a uma condição especificada.
- DEFAULT: Define um valor padrão para uma coluna.
- PRIMARY KEY: Define a chave primária da tabela, garantindo que os valores sejam únicos e não nulos.
- FOREIGN KEY: Define uma chave estrangeira que estabelece uma relação com outra tabela.
- UNIQUE: Define uma restrição para garantir que os valores em uma coluna sejam exclusivos.

## Coluna:
- ADD COLUMN: Adiciona uma nova coluna a uma tabela existente.
- ALTER COLUMN: Modifica a definição de uma coluna existente em uma tabela.
- DROP COLUMN: Remove uma coluna de uma tabela existente.

## Manipulação de Dados:
- INSERT INTO: Insere novos registros em uma tabela.
- INSERT INTO SELECT: Insere registros selecionados de uma tabela em outra.
- VALUES: Especifica os valores a serem inseridos em uma tabela em uma consulta INSERT.
- UPDATE: Modifica os valores de uma ou mais colunas em registros existentes em uma tabela.
- DELETE: Remove registros de uma tabela.

## Seleção de Dados:
- SELECT: Recupera dados de uma ou mais tabelas.
- FROM: Especifica a tabela ou tabelas a partir das quais os dados serão recuperados na consulta.
- SELECT DISTINCT: Recupera valores exclusivos de uma coluna em uma consulta.
- SELECT INTO: Seleciona dados de uma tabela existente e os insere em uma nova tabela.
- SELECT TOP: Limita o número de registros retornados em uma consulta.

## Índice:
- CREATE INDEX: Cria um índice para acelerar a consulta de dados em uma tabela.
- CREATE UNIQUE INDEX: Cria um índice único para garantir que os valores em uma coluna sejam exclusivos.
- DROP INDEX: Remove um índice existente.

## Visão (View):
- CREATE VIEW: Cria uma visão (uma consulta armazenada) com base em uma ou mais tabelas.
- CREATE OR REPLACE VIEW: Cria uma nova visão ou substitui uma existente se já existir.
- ALTER VIEW: Modifica a definição de uma visão existente.
- DROP VIEW: Exclui uma visão existente.

## Filtragem de Dados:
- WHERE: Filtra os registros com base em uma condição especificada.
- AND: Operador lógico "E" que combina múltiplas condições.
- OR: Operador lógico "OU" que combina múltiplas condições.
- NOT: Operador lógico de negação.
- IN: Verifica se um valor está presente em uma lista de valores.
- LIKE: Utilizado para pesquisar padrões em strings.
- BETWEEN: Verifica se um valor está dentro de um intervalo.
- EXISTS: Verifica se a subconsulta retorna algum resultado.
- IS NULL: Verifica se um valor é nulo.
- IS NOT NULL: Verifica se um valor não é nulo.

## Expressões:
- CASE: Permite realizar operações condicionais em uma consulta.

## Operadores:
- Aritméticos: +, -, *, /, %
- Comparação: =, <>, >, <, >=, <=
- Lógicos: AND, OR, NOT
- Concatenação de strings: +
- IN: Verifica se um valor está presente em uma lista de valores.
- BETWEEN: Verifica se um valor está dentro de um intervalo.
- LIKE: Utilizado para pesquisar padrões em strings.

## Ordenação de Resultados:
- ORDER BY: Ordena os resultados com base em uma ou mais colunas.

## Agrupamento e Agrupamento com Filtro:
- GROUP BY: Agrupa os resultados com base em uma ou mais colunas.
- HAVING: Filtra os grupos com base em uma condição após o uso do GROUP BY.

## Limitação de Resultados:
- LIMIT (para MySQL e PostgreSQL): Limita o número de registros retornados em uma consulta.
- ROWNUM (para Oracle): Limita o número de registros retornados em uma consulta.
- TOP (para SQL Server): Limita o número de registros retornados em uma consulta.

## Comandos de Conjunto (Set):
- UNION: Combina os resultados de duas ou mais consultas, retornando apenas registros distintos (sem duplicatas).
- UNION ALL: Combina os resultados de duas ou mais consultas, retornando todos os registros, inclusive os duplicados.
- INTERSECT: Retorna apenas os registros que estão presentes em ambas as consultas.
- MINUS (ou EXCEPT em alguns bancos de dados): Retorna os registros da primeira consulta que não estão presentes na segunda consulta.

## Funções:
- Funções de Agregação (Aggregate Functions):
  - COUNT: Retorna o número de linhas ou valores não nulos em uma coluna.
  - SUM: Retorna a soma dos valores em uma coluna numérica.
  - AVG: Retorna a média dos valores em uma coluna numérica.
  - MAX: Retorna o maior valor em uma coluna.
  - MIN: Retorna o menor valor em uma coluna.
- Funções de Texto (String Functions):
  - CONCAT: Concatena duas ou mais strings.
  - SUBSTRING: Extrai uma parte de uma string com base em uma posição e comprimento específicos.
  - LENGTH: Retorna o número de caracteres em uma string.
  - UPPER / LOWER: Converte uma string para maiúsculas ou minúsculas.
- Funções de Data e Hora (Date and Time Functions):
  - DATEADD: Adiciona um intervalo de tempo a uma data ou hora.
  - DATEDIFF: Retorna a diferença entre duas datas ou horas.
  - GETDATE / CURRENT_TIMESTAMP: Retorna a data e hora atual do sistema.
  - DATEPART: Retorna uma parte específica (ano, mês, dia, hora, etc.) de uma data ou hora.
- Funções de Conversão de Dados (Data Conversion Functions):
  - CAST: Converte um valor de um tipo de dados para outro.
  - CONVERT: Converte um valor de um tipo de dados para outro (específico para alguns bancos de dados).
- Funções Matemáticas:
  - ABS: Retorna o valor absoluto de um número.
  - ROUND: Arredonda um número para um determinado número de casas decimais.
  - CEIL / CEILING: Arredonda um número para cima.
  - FLOOR: Arredonda um número para baixo.
  - SQRT: Retorna a raiz quadrada de um número.
- Funções Lógicas:
  - IF / CASE: Permite realizar operações condicionais em uma consulta.
  - COALESCE: Retorna o primeiro valor não nulo de uma lista de valores.
  - NULLIF: Retorna nulo se dois valores forem iguais; caso contrário, retorna o primeiro valor.