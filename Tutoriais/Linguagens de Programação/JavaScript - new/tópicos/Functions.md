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
  O operador spread `...` em parâmetros é uma ferramenta útil para lidar com um número variável de argumentos em funções, transformando-os em um array de elementos. No entanto, é importante notar que, uma vez utilizado o operador spread, não é possível colocar parâmetros adicionais após ele.

  ```javascript
  1 function somatorio(...valores) {
  2   // soma de todos os valores dentro da variável valores
  3 }
  ```
  No exemplo acima, a função `somatorio` utiliza o operador spread para coletar todos os valores fornecidos durante a chamada, representados pelo parâmetro `valores`.

  Dentro do corpo da função, podemos realizar operações, como calcular a soma de todos os valores, graças à capacidade do operador spread de transformar esses argumentos em um array. É crucial notar que, após o uso do operador spread, não é possível incluir parâmetros adicionais na função, já que ele deve ser o último na lista de parâmetros.

  ### Retorno da Função
  O retorno de uma função em JavaScript refere-se ao valor que a função produz ou "devolve" após sua execução. Isso permite que você utilize o resultado da função em outras partes do seu código.

  ```Javascript
  1 function somar(a, b) {
  2   return a + b;
  3 }
  ```

  No exemplo acima, temos uma função chamada `somar` (linha 1) que recebe dois parâmetros (`a` e `b`) e retorna a soma desses dois valores. A instrução `return` (linha 2) é usada para indicar o valor que a função deve retornar.


## Chamada de Funções
A eficácia da programação em JavaScript está intimamente ligada à habilidade de chamar funções de maneira precisa e flexível. Este processo abrange três aspectos cruciais:
  ### Como Chamar uma Função
  Chamar uma função em JavaScript é uma ação fundamental que invoca a execução do bloco de código associado a essa função. A sintaxe básica envolve escrever o nome da função seguido por parênteses. Se a função aceitar parâmetros, esses valores específicos são fornecidos dentro dos parênteses durante a chamada.

  ```javascript
  1 function saudacao(nome) {
  2   console.log(`Olá, ${nome}!`);
  3 }
  4
  5 saudacao("Alice"); // Saída: Olá, Alice!
  ```

  No exemplo acima, a função `saudacao` é chamada com o argumento "Alice", que é passado para o parâmetro `nome`. O bloco de código dentro da função é então executado, produzindo a saudação personalizada.

  ### Argumentos em Chamadas de Função
  Os argumentos são os valores fornecidos durante a chamada de uma função e são atribuídos aos parâmetros correspondentes dentro do escopo da função. JavaScript permite que você forneça diferentes tipos e quantidades de argumentos, dependendo da definição da função.

  ```javascript
  1 function somar(a, b) {
  2   console.log(a + b);
  3 }
  4
  5 somar(3, 4); // Saída: 7
  ```

  Neste exemplo, a função `somar` é chamada com os argumentos `3` e `4`, que são somados dentro da função.

  ### Uso do Operador Spread na Chamada de Funções
  O operador spread (`...`) é uma ferramenta versátil que não só pode ser utilizada na definição de funções, mas também na sua chamada. Ele oferece uma forma concisa e flexível de passar múltiplos argumentos para uma função, especialmente quando esses valores estão armazenados em arrays ou objetos.

  **Exemplo com Array:**
  ```javascript
  1 function adicionarValores(a, b, c) {
  2   console.log(a + b + c);
  3 }
  4
  5 const valores = [1, 2, 3];
  6 adicionarValores(...valores); // Saída: 6
  ```

  Neste exemplo, o operador spread é usado para espalhar os elementos do array `valores` como argumentos individuais durante a chamada da função `adicionarValores`. Essa abordagem simplifica a passagem de argumentos quando eles estão agrupados em um array.

  **Exemplo com Objeto:**
  ```javascript
  1 function exibirDetalhes(nome, idade, cidade) {
  2   console.log(`Nome: ${nome}, Idade: ${idade}, Cidade: ${cidade}`);
  3 }
  4
  5 const pessoa = { nome: "Bob", idade: 30, cidade: "Cityville" };
  6 exibirDetalhes(...Object.values(pessoa)); // Saída: Nome: Bob, Idade: 30 Cidade: Cityville
  ```

  Neste exemplo, o operador spread é combinado com `Object.values` para passar os valores individuais das propriedades do objeto `pessoa` como argumentos para a função `exibirDetalhes`. Isso proporciona uma maneira eficiente de transmitir os valores do objeto como argumentos.

  Em resumo, o uso do operador spread na chamada de funções oferece uma solução clara e eficaz para lidar com múltiplos argumentos, seja em arrays ou objetos, aumentando a flexibilidade e a clareza do código.

## Tipos de Funções
As funções em JavaScript desempenham um papel central na estruturação e organização do código, oferecendo flexibilidade e modularidade. Existem diversos tipos de funções, cada uma com características específicas que se adequam a diferentes necessidades de programação. Vamos explorar alguns dos principais tipos de funções e entender como cada uma delas contribui para a eficácia e expressividade do código.

  ### Função Nomeada
  A função nomeada em JavaScript é caracterizada por ter um nome associado a ela. Esse nome não apenas identifica a função no código, mas também pode ser usado para chamá-la recursivamente ou referenciar a função em diferentes partes do programa.

  ```javascript
  1 function calcularQuadrado(numero) {
  2   return numero * numero;
  3 }
  4
  5 const resultado = calcularQuadrado(5); // Resultado: 25
  ```

  Neste exemplo, `calcularQuadrado` é uma função nomeada que aceita um número como parâmetro e retorna o quadrado desse número.

  ### Função Anônima
  Ao contrário da função nomeada, a função anônima não possui um nome associado. Ela é geralmente definida em tempo de execução e frequentemente atribuída a uma variável ou passada como argumento para outra função.

  ```javascript
  1 const saudacao = function(nome) {
  2   console.log(`Olá, ${nome}!`);
  3 };
  4
  5 saudacao("Alice"); // Saída: Olá, Alice!
  ```

  Neste exemplo, `saudacao` é uma função anônima atribuída à variável. Pode ser chamada da mesma forma que uma função nomeada.

  ### Função de Seta (Arrow Function)
  A função de seta em JavaScript é uma forma mais concisa de declarar funções, introduzida no ECMAScript 6 (ES6). Ela mantém uma sintaxe simplificada e um comportamento específico de escopo em relação à palavra-chave `this`. Uma das características fundamentais é que a função de seta herda o valor de `this` do escopo exterior em que foi criada.

  ```javascript
  1 const dobrar = (numero) => {
  2   return numero * 2;
  3 };
  4
  5 const resultado = dobrar(3); // Resultado: 6
  ```

  Neste exemplo, `dobrar` é uma função de seta que dobra o número passado como argumento.

  ### Função Autoinvocada (IIFE)
  A função autoinvocada, ou IIFE (Immediately Invoked Function Expression), é uma função que é executada imediatamente após ser definida. Ela é útil para criar escopos isolados e evitar poluição do escopo global.

  ```javascript
  1 (function() {
  2   const mensagem = "Esta função é autoinvocada!";
  3   console.log(mensagem);
  4 })();
  ```
  Neste exemplo, a função é definida e invocada imediatamente, protegendo a variável `mensagem` de afetar o escopo global.

## Escopo de Função
O escopo de função é um conceito fundamental em JavaScript que governa a visibilidade e a acessibilidade de variáveis dentro de uma função. Compreender como as variáveis são tratadas no escopo de função e explorar o conceito de closure são aspectos cruciais para desenvolvedores que buscam criar código claro, modular e eficiente.

  ### Variáveis e Escopo
  Em JavaScript, variáveis declaradas dentro de uma função têm um escopo local, o que significa que só são acessíveis dentro dessa função. Essa característica promove a encapsulação e impede conflitos de nomes entre diferentes partes do código.

  ```javascript
  1 function exemploEscopo() {
  2   let mensagem = "Variável local";
  3   console.log(mensagem);
  4 }
  5
  6 exemploEscopo(); // Saída: Variável local
  ```
  Tentar acessar a variável `mensagem` fora da função resultaria em um erro, pois está fora do escopo da função.
  ### Closure
  Closure é um conceito poderoso em JavaScript que se refere à capacidade de uma função acessar variáveis de seu escopo externo, mesmo após a execução da função ter sido concluída. Isso é possível porque a função "lembra" do ambiente em que foi criada, mantendo referências a variáveis externas. Vamos explorar mais profundamente como closure funciona.

  Closure ocorre quando uma função é declarada dentro do corpo de outra função, e a função interna referencia variáveis da função externa. Vejamos um exemplo:

  ```javascript
  1 function criarCumprimento(nome) {
  2   let mensagem = `Olá, ${nome}!`;
  3
  4   function cumprimentar() {
  5     console.log(mensagem);
  6   }
  7
  8   return cumprimentar;
  9 }
  10
  11 const cumprimentarUsuario = criarCumprimento("Alice");
  12 cumprimentarUsuario(); // Saída: Olá, Alice!
  ```

  No exemplo acima, `criarCumprimento` retorna a função `cumprimentar`, e essa função interna ainda tem acesso à variável `mensagem` mesmo após a conclusão da execução de `criarCumprimento`.

  Compreender e saber utilizar closures é fundamental para escrever código JavaScript mais modular, eficiente e seguro. Essa capacidade de criar funções que "lembram" de seus ambientes de criação é uma característica distintiva e poderosa da linguagem.
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