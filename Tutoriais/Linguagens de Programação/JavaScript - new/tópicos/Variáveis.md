# Variáveis

## Sumário
- [O que é uma Variável?](#o-que-é-uma-variável)
- [Declaração de Variável](#declaração-de-variáveis)
  - [Declaração com var](#declaração-com-var)
  - [Declaração com let](#declaração-com-let)
  - [Declaração com const](#declaração-com-const)
- [Atribuição de Valores](#atribuição-de-valores)
  - [Atribuição Simples](#atribuição-simples)
  - [Atribuição Inline](#atribuição-inline)
  - [Atribuição por Desestruturação](#atribuição-por-desestruturação)
    - [Desestruturação de Array](#desestruturação-de-array)
    - [Desestruturação de Object](#desestruturação-de-object)
  - [Atribuição com o Operador Spread](#atribuição-com-o-operador-spread)
- [Escopo de Variáveis](#escopo-de-variáveis)
  - [Escopo Local](#escopo-local)
  - [Escopo de Bloco](#escopo-de-bloco)
  - [Escopo Global](#escopo-global)
- [Içamento (Hoisting)](içamento-(hoisting))
  - [Içamento de Variáveis](#içamento-de-variáveis)
  - [Içamento de Funções](#içamento-de-funções)
- [Variáveis de Referência](#variáveis-de-referência)
- [Clonagem de Dados](#clonagem-de-dados)
  - [Clonagem Superficial](#clonagem-superficial)
  - [Cópia Profunda](#cópia-profunda)
- [Resumo](#resumo)
- [Boas Práticas](#boas-práticas)
- [Referências](#referências)

## O que é uma Variável?
Uma variável em programação é um espaço de armazenamento nomeado que contém dados ou valores manipulados por um programa. Elas são fundamentais para a manipulação e armazenamento temporário de informações durante a execução do código. Cada variável possui um identificador único, permitindo referenciá-la em diferentes partes do programa.

## Declaração de Variáveis
A declaração de variáveis é o processo de criar uma nova variável no programa, especificando seu nome e, opcionalmente, atribuindo um valor inicial. Em JavaScript, existem três maneiras principais de declarar variáveis: `var`, `let` e `const`.

### Declaração com `var`
A palavra-chave `var` foi historicamente usada para declarar variáveis em JavaScript. No entanto, ela tem escopo de função e pode levar a comportamentos inesperados quando usada em blocos, como loops.

```javascript
var numero = 10;
```

### Declaração com `let`
A palavra-chave `let` foi introduzida no ECMAScript 6 (ES6) e é amplamente preferida para declaração de variáveis. Ela possui escopo de bloco, o que significa que a variável é válida apenas dentro do bloco em que foi declarada.

```javascript
let nome = 'Alice';
```

### Declaração com `const`
A palavra-chave `const` é usada para criar variáveis com valores que não podem ser reatribuídos. Isso significa que, uma vez atribuído um valor a uma variável constante, esse valor não pode ser alterado durante a execução do programa.

```javascript
const pi = 3.14;
```

Essas diferentes formas de declarar variáveis em JavaScript oferecem flexibilidade e controle sobre o escopo e a mutabilidade das variáveis, permitindo aos desenvolvedores escolher a abordagem mais adequada para cada situação.

## Atribuição de Valores
A atribuição de valores em JavaScript é uma operação fundamental para associar dados a variáveis ou propriedades de objetos. Vamos explorar algumas formas comuns de realizar essa operação.

### Atribuição Simples
A forma mais direta é a atribuição simples, usando o operador de atribuição (`=`). Aqui está um exemplo:

```javascript
let numero = 42;
```

Neste caso, o valor `42` é atribuído à variável `numero`. Essa forma é simples e amplamente utilizada.

### Atribuição Inline
A atribuição inline é útil quando desejamos declarar e atribuir valores a várias variáveis em uma única linha, economizando espaço e tornando o código mais conciso.

```javascript
let nome = 'Alice', idade = 25, cidade = 'Exemplo City';
```

Este exemplo declara e atribui valores às variáveis `nome`, `idade` e `cidade` na mesma linha.

### Atribuição por Desestruturação
A desestruturação é uma poderosa técnica para extrair valores de arrays ou objetos e atribuí-los a variáveis individuais de maneira concisa.

#### Desestruturação de Array
```javascript
let numeros = [1, 2, 3];
let [a, b, c] = numeros;
console.log(a, b, c); // Resultado: 1 2 3
```

Aqui, os valores do array `numeros` são atribuídos às variáveis `a`, `b` e `c` respectivamente.

#### Desestruturação de Object
```javascript
let pessoa = { nome: 'Bob', idade: 30 };
let { nome, idade } = pessoa;
console.log(nome, idade); // Resultado: Bob 30
```

Neste exemplo, a desestruturação é usada para extrair as propriedades `nome` e `idade` do objeto `pessoa` e atribuí-las a variáveis do mesmo nome.

### Atribuição com o Operador Spread
O operador spread (`...`) é empregado para criar cópias de arrays ou objetos, evitando referências diretas. Vejamos um exemplo:

```javascript
let original = [1, 2, 3];
let copia = [...original];
console.log(copia); // Resultado: [1, 2, 3]
```

Ao utilizar o spread, garantimos que `copia` seja uma cópia independente de `original`, evitando problemas relacionados a referências compartilhadas.

Essas diversas formas de atribuição oferecem flexibilidade e expressividade ao programar em JavaScript, permitindo que os desenvolvedores escolham a abordagem mais adequada para cada contexto.

## Escopo de Variáveis
O escopo de variáveis é um conceito fundamental que determina a visibilidade e acessibilidade de uma variável em um programa JavaScript. Entender os diferentes níveis de escopo é crucial para escrever código claro, modular e livre de conflitos.

### Escopo Local
Quando uma variável é declarada dentro de uma função, ela tem escopo local. Isso significa que só é acessível dentro dessa função específica. Variáveis locais ajudam a encapsular dados, evitando interferências externas.

```javascript
function exemploEscopoLocal() {
  let variavelLocal = 'Esta é uma variável local';
  console.log(variavelLocal);
}

// variavelLocal não é acessível aqui
```

Neste contexto, `variavelLocal` só pode ser utilizada dentro da função `exemploEscopoLocal`, promovendo a segurança e prevenindo conflitos inadvertidos.

### Escopo de Bloco
Com a introdução de `let` e `const` no ECMAScript 6, o escopo de bloco foi introduzido. Agora, variáveis declaradas com essas palavras-chave têm escopo limitado ao bloco em que são definidas.

```javascript
if (true) {
  let variavelBloco = 'Esta é uma variável de bloco';
  console.log(variavelBloco);
}

// variavelBloco não é acessível aqui
```

Dentro do bloco condicional, `variavelBloco` existe, mas fora dele, não. Essa precisão no escopo proporciona uma gestão mais eficaz de variáveis.

### Escopo Global
Variáveis declaradas fora de funções ou blocos têm escopo global, tornando-as acessíveis em todo o código. No entanto, seu uso excessivo pode levar a problemas de legibilidade e manutenção.

```javascript
let variavelGlobal = 'Esta é uma variável global';

function exemploEscopoGlobal() {
  console.log(variavelGlobal);
}

exemploEscopoGlobal(); // A variável global é acessível aqui
```

Variáveis globais devem ser usadas com cuidado, pois podem ser modificadas de maneiras inesperadas, impactando o código em diversos pontos.

Entender o escopo de variáveis é uma habilidade essencial para desenvolvedores JavaScript. Esse entendimento permite a criação de código mais modular, seguro e fácil de manter, contribuindo para o desenvolvimento de software robusto e eficiente.

## Içamento (Hoisting)
O içamento, ou hoisting em inglês, é um comportamento peculiar do JavaScript em que declarações de variáveis e funções são "elevadas" para o topo do contexto de execução durante a fase de compilação. Compreender esse conceito é essencial para evitar comportamentos inesperados no código.

### Içamento de Variáveis
No içamento de variáveis, a declaração é movida para o topo do escopo, enquanto a atribuição permanece no local original. É importante notar que `let` e `const` são içadas, mas não são inicializadas durante essa fase. Isso cria uma "zona morta temporal" em que essas variáveis não podem ser acessadas antes da sua declaração.

```javascript
console.log(nome); // Saída: undefined
var nome = 'Alice';

console.log(outraVariavel); // Erro: outraVariavel is not defined
let outraVariavel = 'Bob';
```

No exemplo acima, a variável `nome` é içada e inicializada com `undefined` (comportamento de `var`), mas a tentativa de acessar `outraVariavel` antes da sua declaração resulta em um erro de "zona morta temporal".

### Içamento de Funções
O içamento de funções funciona de maneira semelhante. A declaração da função é movida para o topo, permitindo que ela seja chamada antes mesmo de ser declarada no código.

```javascript
saudacao(); // Saída: Olá!

function saudacao() {
  console.log('Olá!');
}
```

Aqui, a função `saudacao` pode ser chamada antes da sua declaração no código, graças ao içamento de funções.

Entender o içamento é crucial para evitar comportamentos inesperados e escrever um código mais previsível e legível. Ao conhecer como o JavaScript lida com o içamento, os desenvolvedores podem tomar decisões mais informadas sobre a organização e estrutura do código.

## Variáveis de Referência
Em JavaScript, variáveis de referência, como objetos e arrays, não armazenam diretamente os dados, mas sim um endereço de memória que aponta para a localização dos dados. Isso significa que, ao atribuir uma variável a outra, estamos, na verdade, copiando a referência, não os dados em si.

```javascript
let originalArray = [1, 2, 3];
let novaArray = originalArray;

novaArray.push(4);

console.log(originalArray); // Resultado: [1, 2, 3, 4]
```

Neste exemplo, ao modificar `novaArray`, a variável `originalArray` também é afetada. Isso ocorre porque ambas compartilham a mesma referência ao array na memória.

## Clonagem de Dados
Ao lidar com objetos ou arrays em JavaScript, a clonagem de dados é uma prática importante para garantir a integridade dos dados e evitar efeitos colaterais inesperados.

### Clonagem Superficial
Para evitar o compartilhamento indesejado de referências, podemos recorrer à clonagem superficial usando o operador spread (`...`).

```javascript
let originalArray = [1, 2, 3];
let cloneArray = [...originalArray];

cloneArray.push(4);

console.log(originalArray); // Resultado: [1, 2, 3]
console.log(cloneArray);   // Resultado: [1, 2, 3, 4]
```

A clonagem superficial cria uma cópia independente dos dados, impedindo que alterações em uma variável afetem a outra. Essa estratégia é especialmente útil para arrays simples.

### Cópia Profunda
A cópia profunda é uma estratégia de clonagem que cria uma cópia totalmente independente de uma estrutura de dados, garantindo que quaisquer alterações feitas na cópia não afetem o objeto original. Essa técnica é especialmente crucial ao lidar com objetos aninhados ou estruturas complexas, onde a clonagem superficial pode não ser suficiente para garantir a separação completa entre as variáveis. Em JavaScript, bibliotecas como o Lodash fornecem métodos, como `cloneDeep`, para realizar cópias profundas de objetos, assegurando uma total independência entre as instâncias clonadas e originais.

Outras técnicas serão abordadas em temas posteriores, como Arrays e Objetos.

Compreender variáveis de referência e técnicas de clonagem é fundamental para desenvolver código robusto em JavaScript. Esses conceitos possibilitam o gerenciamento eficiente de dados, evitando efeitos colaterais indesejados e garantindo a integridade das estruturas de dados.

## Resumo Enriquecido

- ### **O que é uma Variável?**
  - Uma variável em JavaScript é um contêiner nomeado para armazenar dados. Esses dados podem ser modificados e referenciados durante a execução do programa.

- ### **Declaração de Variáveis**
  - **Declaração com var:**
    - Forma mais antiga de declarar variáveis, com escopo de função e sujeita a içamento.
  - **Declaração com let:**
    - Introduzida no ECMAScript 6, oferece escopo de bloco e evita o içamento.
  - **Declaração com const:**
    - Cria uma variável de valor constante, não reatribuível, com escopo de bloco.

- ### **Atribuição de Valores**
  - **Atribuição Simples:**
    - Atribui um valor a uma variável de forma direta.
  - **Atribuição Inline:**
    - Declara e atribui valor à variável em uma única linha.
  - **Atribuição por Desestruturação:**
    - Extrai valores de arrays e objetos de maneira concisa.
    - **Desestruturação de Array**
    - **Desestruturação de Object**
  - **Atribuição com o Operador Spread:**
    - Espalha elementos de um objeto ou array em outro.

- ### **Escopo de Variáveis**
  - **Escopo Local:**
    - Variáveis dentro de funções têm escopo local.
  - **Escopo de Bloco:**
    - Variáveis com `let` e `const` têm escopo restrito ao bloco.
  - **Escopo Global:**
    - Variáveis fora de funções têm escopo global.

- ### **Içamento (Hoisting)**
  - **Içamento de Variáveis:**
    - Declarações de variáveis movidas para o topo de seu contexto de execução.
  - **Içamento de Funções:**
    - Declarações de funções movidas para o topo de seu contexto de execução.

- ### **Variáveis de Referência**
  - Variáveis que armazenam referências a objetos em vez de valores diretamente.

- ### **Clonagem de Dados**
  - **Clonagem Superficial:**
    - Cria uma cópia superficial de um objeto.
  - **Cópia Profunda:**
    - Cria uma cópia completa de um objeto, incluindo objetos aninhados.

Vamos criar uma lista de boas práticas e observações para os tópicos fornecidos:

## Boas Práticas e Observações para Variáveis em JavaScript

### O que é uma Variável?

1. **Conceito de Variável:**
   - Entenda que variáveis são espaços de armazenamento para dados e podem ser nomeadas conforme a necessidade do programador.

### Declaração de Variáveis

1. **Declaração com `var`:**
   - Evite o uso de `var` para declaração de variáveis devido ao seu escopo de função, que pode causar problemas de vazamento de variáveis.

2. **Declaração com `let`:**
   - Prefira `let` para declarar variáveis que precisam de escopo de bloco, proporcionando uma melhor estruturação do código.

3. **Declaração com `const`:**
   - Utilize `const` para declarar variáveis cujo valor não será reatribuído. Isso promove a imutabilidade e a prevenção de erros.

### Atribuição de Valores

1. **Atribuição Simples:**
   - Realize atribuições de valores de forma clara, evitando redundâncias e garantindo legibilidade.

2. **Atribuição Inline:**
   - Ao declarar e atribuir valores, considere a atribuição inline quando a inicialização da variável ocorre na mesma linha.

3. **Atribuição por Desestruturação:**
   - Explore a desestruturação de arrays e objetos para atribuir valores de maneira concisa.

   - **Desestruturação de Array:**
      - Atribua valores a partir de um array para variáveis individuais usando a desestruturação.

   - **Desestruturação de Object:**
      - Extraia valores de propriedades de objetos usando a desestruturação.

4. **Atribuição com o Operador Spread:**
   - Utilize o operador spread para clonar e expandir arrays ou objetos durante a atribuição de valores.

### Escopo de Variáveis

1. **Escopo Local:**
   - Opte por escopo local sempre que possível, limitando a visibilidade da variável ao bloco ou à função onde é declarada.

2. **Escopo de Bloco:**
    - Dê preferência a `let` e `const` para aproveitar o escopo de bloco, especialmente em estruturas condicionais e loops.

3. **Escopo Global:**
    - Minimize o uso de variáveis globais para evitar conflitos e garantir uma melhor modularidade.

### Içamento (Hoisting)

1. **Içamento de Variáveis:**
    - Esteja ciente do comportamento de içamento (`hoisting`) em variáveis declaradas com `var`. Declare as variáveis no início do escopo para evitar comportamentos inesperados.

12. **Içamento de Funções:**
    - Compreenda o içamento de funções e declare funções antes de utilizá-las para evitar problemas de referência.

### Variáveis de Referência

1. **Conhecimento de Variáveis de Referência:**
    - Esteja ciente de que as variáveis de objetos e arrays armazenam referências, o que pode levar a efeitos colaterais se não gerenciadas corretamente.

### Clonagem de Dados
1. **Clonagem Superficial:**
    - Ao clonar objetos ou arrays, compreenda a diferença entre clonagem superficial e clonagem profunda. Considere o uso de métodos apropriados.

2. **Cópia Profunda:**
    - Utilize técnicas adequadas para realizar cópias profundas de objetos e arrays, garantindo que as estruturas internas também sejam clonadas.

## Referências
- **JavaScript.Info**:
  - [Variáveis](https://javascript.info/variables)
  - [Escopo](https://javascript.info/closure)
- **W3Schools**:
  - [Variáveis](https://www.w3schools.com/js/js_variables.asp)
  - [Let](https://www.w3schools.com/js/js_let.asp)
  - [Const](https://www.w3schools.com/js/js_const.asp)
  - [Escopo](https://www.w3schools.com/js/js_scope.asp)