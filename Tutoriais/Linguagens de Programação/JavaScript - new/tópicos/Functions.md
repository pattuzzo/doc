Funções
Introdução às Funções
  O que é uma Função?
  Sintaxe Básica
  Declaração
  Parâmetros e Valores Padrão
  Operador Spread em Parâmetros
  Retorno da Função
Chamada de Funções
  Como Chamar uma Função
  Argumentos em Chamadas de Função
  Uso do Operador Spread na Chamada de Funções
Tipos de Funções
  Função Nomeada
  Função Anônima
  Função de Seta (Arrow Function)
  Função Autoinvocada (IIFE)
Escopo de Função
  Variáveis e Escopo
  Closure
Técnicas Avançadas de Funções
  Recursividade
  Callbacks
  Funções de Ordem Superior
Construtores de Função e Protótipos
  Declaração de Construtores de Função
  Utilização de Protótipos
Resumo
- Introdução às Funções
  resumo
- Chamada de Funções
  resumo
- Tipos de Funções
  - Função Nomeada
  - Função Anônima
  - Função de Seta (Arrow Function)
  - Função Autoinvocada (IIFE)
- Escopo de Função
  resumo
- Técnicas Avançadas
  - Recursividade
  - Callbacks
  - Funções de Ordem Superior
- Construtores de Função e Protótipos
  resumo
Boas Práticas
Referências





# Funções

## Sumário
- [Introdução às Funções](#introdução-às-funções)
  - [O que é uma Função?](#o-que-é-uma-função)
  - [Sintaxe Básica](#sintaxe-básica)
  - [Parâmetros e Valores Padrão](#parâmetros-e-valores-padrão)
  - [Operador Spread em Parâmetros](#operador-spread-em-parâmetros)
  - [Retorno da Função](#retorno-da-função)
- [Chamada de Funções](#chamada-de-funções)
  - [Como Chamar uma Função](#como-chamar-uma-função)
  - [Argumentos em Chamadas de Função](#argumentos-em-chamadas-de-função)
  - [Uso do Operador Spread na Chamada de Funções](#uso-do-operador-spread-na-chamada-de-funções)
- [Tipos de Funções](#tipos-de-funções)
  - [Função Nomeada](#função-nomeada)
  - [Função Anônima](#função-anônima)
  - [Função de Seta (Arrow Function)](#função-de-seta-arrow-function)
  - [Função Autoinvocada (IIFE)](#função-autoinvocada-iife)
- [Escopo de Função](#escopo-de-função)
  - [Variáveis e Escopo](#variáveis-e-escopo)
  - [Closure](#closure)
- [Técnicas Avançadas de Funções](#técnicas-avançadas-de-funções)
  - [Recursividade](#recursividade)
  - [Callbacks](#callbacks)
  - [Funções de Ordem Superior](#funções-de-ordem-superior)
- [Construtores de Função e Protótipos](#construtores-de-função-e-protótipos)
  - [Declaração de Construtores de Função](#declaração-de-construtores-de-função)
  - [Utilização de Protótipos](#utilização-de-protótipos)
- [Resumo](#resumo)
  - [Introdução às Funções](#introdução-às-funções-resumo)
  - [Chamada de Funções](#chamada-de-funções-resumo)
  - [Tipos de Funções](#tipos-de-funções-resumo)
  - [Escopo de Função](#escopo-de-função-resumo)
  - [Técnicas Avançadas](#técnicas-avançadas-resumo)
  - [Construtores de Função e Protótipos](#construtores-de-função-e-protótipos-resumo)
- [Boas Práticas](#boas-práticas)
- [Referências](#referências)

## Introdução às Funções
Introdução às Funções em JavaScript

JavaScript, como uma linguagem de programação versátil e amplamente utilizada, oferece uma poderosa ferramenta para estruturar e organizar o código: as funções. Estas desempenham um papel fundamental no desenvolvimento de aplicações, permitindo a modularização, reutilização e manutenção eficiente do código.

Neste contexto, é essencial compreender não apenas a sintaxe básica das funções, mas também seus diversos tipos e aplicações. Desde funções nomeadas até as modernas funções de seta (Arrow Functions), cada uma tem sua utilidade específica e contribui para a expressividade e eficácia do código JavaScript.

Além disso, exploraremos aspectos cruciais como escopo de função, closures e técnicas avançadas, incluindo recursividade, callbacks e funções de ordem superior. Ao compreender esses conceitos, os desenvolvedores podem elevar seu domínio sobre JavaScript, aproveitando ao máximo suas capacidades.

Por fim, abordaremos construtores de função e protótipos, fundamentais para a criação de objetos e estruturas de dados mais complexas. Ao dominar esses elementos, os desenvolvedores estarão preparados para construir aplicações robustas e eficientes em JavaScript.

Vamos mergulhar nesse universo fascinante das funções em JavaScript e desvendar as práticas que impulsionam o desenvolvimento de software moderno.

  ### O que é uma Função?
  Uma função em JavaScript é um bloco de código reutilizável, projetado para realizar uma tarefa específica ou calcular um valor. Ela desencadeia uma ação quando chamada e pode aceitar dados, conhecidos como parâmetros, para personalizar seu comportamento. As funções desempenham um papel crucial na estruturação e organização do código, permitindo que programadores modularizem suas aplicações.
  
  ### Sintaxe Básica
  A Sintaxe Básica de uma função em JavaScript define a estrutura fundamental para criar blocos de código reutilizáveis. Inicia-se com a palavra-chave `function`, seguida pelo nome da função, parênteses (que podem conter parâmetros) e um bloco de código delimitado por chaves. Este bloco de código é executado quando a função é chamada, permitindo modularizar o código para facilitar a manutenção e compreensão.
  ```javascript
  1 function label(parâmetros) {
  2   return valor;
  3 }
  ```
  `function`: Palavra-chave que declara uma função
  `label`: Nome personalizável que identifica a função
  `parâmetros`: Lista de parâmetros (opcionais) aceitos pela função
  `return`: Palavra-chave utilizada para retornar um valor da função

  ### Parâmetros e Valores Padrão
  Em JavaScript, ao trabalhar com funções, é comum lidar com parâmetros, que são os valores que você passa para uma função quando a chama. Os parâmetros são essenciais para que as funções possam aceitar dados externos e realizar operações com esses dados dentro do escopo da função.

  Além disso, para tornar o código mais flexível e robusto, JavaScript oferece suporte a valores padrão para parâmetros de função. Os valores padrão permitem que você atribua valores predefinidos aos parâmetros, garantindo que, se um argumento correspondente não for fornecido durante a chamada da função, o parâmetro terá um valor padrão automaticamente.

  ```javascript
  1 function calcularPotencia(base, expoente = 2) {
  2   return Math.pow(base, expoente);
  3 }

  ```
  Neste exemplo, a função `calcularPotencia` possui dois parâmetros, `base` e `expoente`. O `expoente` tem um valor padrão de `2`. Isso significa que, se o segundo argumento não for fornecido durante a chamada da função, ele será automaticamente assumido como `2`.

  ### Operador Spread em Parâmetros
  O operador spread `...` em parâmetros é uma ferramenta útil para lidar com um número variável de argumentos em funções, transformando-os em uma lista de elementos. No entanto, é importante notar que, uma vez utilizado o operador spread, não é possível colocar parâmetros adicionais após ele.

  ```javascript
  1 function somatorio(...valores) {
  2   // soma de todos os valores dentro da variável valores
  3 }
  ```
  No exemplo acima, a função `somatorio` utiliza o operador spread para coletar todos os valores fornecidos durante a chamada, representados pelo parâmetro `valores`.

  Dentro do corpo da função, podemos realizar operações, como calcular a soma de todos os valores, graças à capacidade do operador spread de transformar esses argumentos em uma lista. É crucial notar que, após o uso do operador spread, não é possível incluir parâmetros adicionais na função, já que ele deve ser o último na lista de parâmetros.

  ### Retorno da Função
  O retorno de uma função em JavaScript refere-se ao valor que a função produz ou "devolve" após sua execução. Isso permite que você utilize o resultado da função em outras partes do seu código.

  ```Javascript
  1 function somar(a, b) {
  2   return a + b;
  3 }
  4
  5 let resultadoSoma = somar(5, 3);
  ```

  No exemplo acima, temos uma função chamada `somar` (linha 1) que recebe dois parâmetros (`a` e `b`) e retorna a soma desses dois valores. A instrução `return` (linha 2) é usada para indicar o valor que a função deve retornar. Quando a função é chamada com `somar(5, 3)` (linha 5), o resultado é 8, que é então atribuído à variável `resultadoSoma`.

## Chamada de Funções
  ### Como Chamar uma Função
  ### Argumentos em Chamadas de Função
  ### Uso do Operador Spread na Chamada de Funções
## Tipos de Funções
  ### Função Nomeada
  ### Função Anônima
  ### Função de Seta (Arrow Function)
  ### Função Autoinvocada (IIFE)
## Escopo de Função
  ### Variáveis e Escopo
  ### Closure
## Técnicas Avançadas de Funções
  ### Recursividade
  ### Callbacks
  ### Funções de Ordem Superior
## Construtores de Função e Protótipos
  ### Declaração de Construtores de Função
  ### Utilização de Protótipos
## Resumo
- ### Introdução às Funções
  resumo
- ### Chamada de Funções
  resumo
- ### Tipos de Funções
  - Função Nomeada: resumo
  - Função Anônima: resumo
  - Função de Seta (Arrow Function): resumo
  - Função Autoinvocada (IIFE): resumo
- ### Escopo de Função
  resumo
- ### Técnicas Avançadas
  - Recursividade: resumo
  - Callbacks: resumo
  - Funções de Ordem Superior: resumo
- ### Construtores de Função e Protótipos
  resumo
## Boas Práticas

## Referências
- [Funções - W3School](https://www.w3schools.com/js/js_function_definition.asp)
- [Funções - JavaScript.info](https://javascript.info/function-basics)