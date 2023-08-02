# TypeScript

## Sumário:
  - [Introdução](#introdução)
  - [História](#história)
  - [Por quê TypeScript?](#por-quê-typescript)
  - [Características](#características)
  - [Instalação](#instalação)
    - [Windows](#windows)
    - [Linux](#linux)
    - [MacOS](#macos)
    - [Web](#web)
  - [Primeiros Passos](#primeiros-passos)
  - [Sintaxe](#sintaxe)
  - [Tipos Básicos](#tipos-básicos)
    - [Number](#number)
    - [String](#string)
    - [Boolean](#boolean)
  - [Tipos Especiais](#tipos-especiais)
    - [Null](#null)
    - [Undefined](#undefined)
    - [Void](#void)
    - [Never](#never)
  - [Tipos Compostos](#tipos-compostos)
    - [Object](#object)
    - [Array](#array)
    - [Tuple](#tuple)
    - [Enum](#enum)
  - [Tipos Genéricos](#tipos-genéricos)
    - [Any](#any)
    - [Unknown](#unknown)
  - [Tipos Avançados](#tipos-avançados)
    - [Tipo Literal](#tipo-literal)
    - [Interface](#interface)
    - [Tipo Alias](#tipo-alias)
    - [União de Tipos](#união-de-tipos)
    - [Intersecção de Tipos](#intersecção-de-tipos)
    - [Tipos Genéricos](#tipos-genéricos)
    - [Inferência de Tipos](#inferência-de-tipos)
  - [Referências](#referências)

## Introdução

TypeScript é uma linguagem de programação desenvolvida pela Microsoft que se baseia em JavaScript, porém adiciona recursos de tipagem estática ao código. A tipagem estática permite que os desenvolvedores especifiquem o tipo das variáveis, parâmetros e retornos de função durante o desenvolvimento, o que ajuda a capturar erros em tempo de compilação e melhora a manutenibilidade e robustez do código.

Esta documentação tem como objetivo fornecer uma visão abrangente dos tipos em TypeScript, abordando desde os tipos básicos até os tipos avançados. É destinada a estudantes e programadores que desejam aprender ou aprofundar seus conhecimentos em TypeScript e como trabalhar com diferentes tipos.

## História

TypeScript foi criado por Anders Hejlsberg, o mesmo criador do C#, e foi lançado inicialmente em outubro de 2012. A linguagem surgiu como uma resposta às limitações da tipagem dinâmica do JavaScript, que muitas vezes levava a erros difíceis de detectar durante o desenvolvimento.

O TypeScript foi projetado para ser um superconjunto de JavaScript, o que significa que qualquer código JavaScript válido também é válido em TypeScript. No entanto, o TypeScript adiciona recursos extras que o tornam uma linguagem de programação mais poderosa e segura, especialmente para projetos grandes e complexos.

## Por quê TypeScript?

O uso do TypeScript oferece diversas vantagens significativas em relação ao JavaScript puro. Algumas das principais razões para utilizar o TypeScript incluem:

1. **Tipagem Estática**: Com a tipagem estática do TypeScript, é possível definir tipos para variáveis, parâmetros e retornos de função. Isso ajuda a evitar erros comuns em tempo de compilação, tornando o código mais confiável.

2. **Intellisense**: O TypeScript oferece suporte a um recurso chamado "Intellisense", que é uma forma avançada de autocompletar no ambiente de desenvolvimento. Isso melhora a produtividade do desenvolvedor, mostrando sugestões de código com base nos tipos definidos.

3. **Melhor Documentação**: A tipagem explícita no TypeScript torna o código mais legível e autoexplicativo, facilitando a compreensão do código para outros desenvolvedores.

4. **Refatoração Segura**: Com a tipagem estática, é mais seguro realizar refatorações no código, pois o TypeScript pode detectar possíveis problemas de tipos e fornecer informações úteis durante o processo de refatoração.

5. **Maior Escalabilidade**: O TypeScript é especialmente útil em projetos grandes e complexos, onde a tipagem estática ajuda a manter o controle sobre o código e reduz a probabilidade de erros inesperados.

6. **Ecossistema JavaScript**: O TypeScript é compatível com o vasto ecossistema de bibliotecas e frameworks JavaScript existentes, permitindo que os desenvolvedores aproveitem o rico conjunto de ferramentas disponíveis.

7. **Suporte para ECMAScript**: O TypeScript é frequentemente atualizado para oferecer suporte às últimas versões do ECMAScript, permitindo que os desenvolvedores usem as mais recentes funcionalidades da linguagem JavaScript.

## Características:
- **Tipagem Estática:** Definição de tipos para variáveis, parâmetros e retornos de funções.
- **Interfaces:** Definição de estruturas de dados com tipos nomeados para promover o reuso e a organização do código.
- **Classes:** Suporte a programação orientada a objetos com classes, herança e encapsulamento.
- **Enumerações:** Criação de conjuntos nomeados de constantes.
- **Generics:** Permite criar componentes reutilizáveis com tipos genéricos.
- **Modificadores de Acesso:** Controle da visibilidade de membros de classes e interfaces.
- **Decoradores:** Anotações aplicadas a classes, métodos e propriedades para extender o comportamento do código.
- **Namespace:** Agrupamento lógico de código para evitar conflitos de nomenclatura.

## Instalação:
Antes de começar a trabalhar com TypeScript, é necessário ter o Node.js instalado em seu sistema. O TypeScript pode ser instalado globalmente via npm ou yarn com o seguinte comando:

```
npm install -g typescript
```

ou

```
yarn global add typescript
```

### Windows:
- Para desenvolvimento no Windows, é recomendado o uso do Visual Studio Code como editor de código.

### Linux:
- No Linux, o Visual Studio Code também é uma excelente opção para desenvolvimento em TypeScript.

### MacOS:
- No MacOS, o Visual Studio Code ou o Xcode podem ser usados para desenvolver em TypeScript.

### Web:
- Caso não queira instalar localmente, é possível utilizar o TypeScript diretamente no navegador através de um Playground online.

## Primeiros Passos:
Após a instalação, crie um arquivo com a extensão ".ts" e comece a escrever código TypeScript. Veja um exemplo simples:

```typescript
// Definindo uma variável com tipagem
let message: string = "Olá, TypeScript!";
console.log(message);

// Função com parâmetro e retorno tipados
function soma(a: number, b: number): number {
  return a + b;
}

// Chamando a função
console.log(soma(5, 3)); // Saída: 8
```

## Sintaxe

Em TypeScript, a sintaxe para a definição de tipos é baseada em anotações que indicam o tipo de uma variável, parâmetro ou retorno de função. Para declarar o tipo de uma variável, usamos o símbolo de dois pontos seguido do tipo desejado.

```typescript
// Exemplo de declaração de variável com tipo
let idade: number;
let nome: string;
let isAdmin: boolean;
```

Para funções, a definição do tipo de parâmetros e retorno é realizada da seguinte forma:

```typescript
// Exemplo de função com tipos
function somar(a: number, b: number): number {
  return a + b;
}
```

## Tipos Básicos

Os tipos básicos em TypeScript representam os tipos primitivos do JavaScript e incluem `number`, `string` e `boolean`. Vamos examinar cada um deles em detalhes:

### Number

O tipo `number` é usado para representar números inteiros ou de ponto flutuante. Em TypeScript, todos os números são do tipo `number`, independentemente de serem inteiros ou de ponto flutuante.

```typescript
let idade: number = 30;
let altura: number = 1.75;
```

### String

O tipo `string` é usado para representar sequências de caracteres (texto). As strings devem ser declaradas entre aspas simples ou duplas.

```typescript
let nome: string = "João";
let frase: string = 'Olá, mundo!';
```

### Boolean

O tipo `boolean` é usado para representar valores verdadeiros ou falsos (true ou false).

```typescript
let isAdmin: boolean = true;
let isGuest: boolean = false;
```

## Tipos Especiais

Além dos tipos básicos, TypeScript também possui alguns tipos especiais, como `null`, `undefined`, `void` e `never`.

### Null

O tipo `null` é usado para representar um valor nulo (aus

ência de valor). Ele é frequentemente usado para indicar que uma variável não possui um valor válido.

```typescript
let valor: number | null = null;
```

### Undefined

O tipo `undefined` é usado para representar um valor não definido. Quando uma variável é declarada, mas não inicializada, ela possui o valor `undefined`.

```typescript
let variavelIndefinida: undefined = undefined;
```

### Void

O tipo `void` é usado principalmente para representar que uma função não possui um valor de retorno. Quando uma função é declarada com o tipo `void`, ela não pode retornar nenhum valor.

```typescript
function exibirMensagem(): void {
  console.log("Olá, mundo!");
}
```

### Never

O tipo `never` é usado para representar um valor que nunca ocorre. Geralmente, é usado para funções que lançam exceções ou entram em loops infinitos, ou para funções que nunca retornam.

```typescript
function lancaExcecao(): never {
  throw new Error("Ocorreu um erro!");
}
```

## Tipos Compostos

Além dos tipos básicos e especiais, TypeScript também oferece tipos compostos que permitem representar estruturas mais complexas de dados.

### Object

O tipo `object` é usado para representar qualquer valor não primitivo. Isso inclui objetos, arrays, funções e qualquer outra coisa que não seja um tipo primitivo.

```typescript
let pessoa: object = { nome: "Alice", idade: 25 };
let numeros: object = [1, 2, 3, 4, 5];
let carro: {marca: string, ano: number} = {marca: "Ford", ano: 2001} // sintaxe alternativa
```

### Array

O tipo `array` é usado para representar uma lista de valores de um determinado tipo. Podemos usar a sintaxe `tipo[]` ou `Array<tipo>` para definir um array.

```typescript
let numeros: number[] = [1, 2, 3, 4, 5];
let nomes: Array<string> = ["Alice", "Bob", "Carol"];
```

### Tuple

Uma tupla é um tipo de array com um número fixo de elementos, onde cada elemento pode ter um tipo diferente. As tuplas são definidas usando colchetes e especificando os tipos dos elementos separados por vírgulas.

```typescript
let pessoa: [string, number] = ["Alice", 25];
```

### Enum

Enum é um tipo que permite associar valores a um conjunto de nomes amigáveis. Isso torna o código mais legível e fácil de entender.

```typescript
enum DiaDaSemana {
  Segunda = 1,
  Terca = 2,
  Quarta = 3,
  Quinta = 4,
  Sexta = 5,
  Sabado = 6,
  Domingo = 7
}

let diaHoje: DiaDaSemana = DiaDaSemana.Sexta;
```

## Tipos Genéricos

Os tipos genéricos permitem criar componentes reutilizáveis e flexíveis, capazes de trabalhar com diferentes tipos de dados.

### Any

O tipo `any` é usado quando o tipo de uma variável ou valor é desconhecido ou quando estamos trabalhando com código JavaScript existente e não queremos fazer uma tipagem rígida.

```typescript
let valor: any = 42;
valor = "Olá";
valor = true;
```

### Unknown

O tipo `unknown` é semelhante ao tipo `any`, mas mais seguro. O tipo `unknown` exige que você faça uma verificação de tipo ou uma conversão explícita antes de trabalhar com o valor.

```typescript
let valor: unknown = 42;

// É necessário fazer uma verificação de tipo antes de utilizar o valor
if (typeof valor === "number") {
  let resultado = valor + 10;
}
```

## Tipos Avançados

Além dos tipos básicos e compostos, TypeScript oferece uma série de tipos avançados que permitem criar estruturas de dados e abstrações mais sofisticadas.

### Tipo Literal

O tipo literal permite definir um tipo que representa um valor específico. Isso é útil em situações onde se quer limitar o conjunto de valores possíveis para uma variável ou parâmetro.

```typescript
let cor: "vermelho" | "azul" | "verde";
cor = "vermelho"; // Válido
cor = "amarelo"; // Inválido, pois "amarelo" não é um valor permitido
```

### Interface

Interfaces são estruturas que descrevem a forma (o formato) que um objeto deve ter em TypeScript. Elas podem ser usadas para descrever a estrutura de um objeto, o formato de uma função e muito mais.

```typescript
interface Carro {
  marca: string;
  ano: number;
}

let carro: Carro = {marca: "BMW", ano: 2016}

interface Pessoa {
  nome: string;
  idade: number;
}

function exibirPessoa(pessoa: Pessoa) {
  console.log(`Nome: ${pessoa.nome}, Idade: ${pessoa.idade}`);
}
```

### Tipo Alias

Os tipos de alias permitem criar um nome personalizado para um tipo existente. Isso é útil para tornar o código mais legível e para reutilizar tipos em várias partes do código.

```typescript
type Coordenada = [number, number];

function moverPara(coord: Coordenada) {
  // Implementação da função
}
```

### União de Tipos

A união de tipos permite que uma variável, parâmetro ou retorno de função possa ter mais de um tipo. Isso é útil quando uma variável pode ter valores de diferentes tipos.

```typescript
function exibirValor(valor: string | number) {
  console.log(`O valor é: ${valor}`);
}
```

### Intersecção de Tipos

A intersecção de tipos permite combinar vários tipos em um único tipo, criando um novo tipo que possui todas as propriedades e características dos tipos originais.

```typescript
interface Animal {
  nome: string;
}

interface Voador {
  voar(): void;
}

type PatoVoador = Animal & Voador;

function mover(pato: PatoVoador) {
  console.log(`${pato.nome} está voando!`);
  pato.voar();
}
```

### Inferência de Tipos

A inferência de tipos é uma característica do TypeScript que permite que o compilador deduza o tipo de uma variável com base no valor atribuído a ela.

```typescript
let numero = 42; // TypeScript inferirá que 'numero' é do tipo 'number'
let nome = "Alice"; // TypeScript inferirá que 'nome' é do tipo 'string'
```

## Referências

1. [TypeScript Documentation](https://www.typescriptlang.org/docs/)
2. [TypeScript Handbook](https://www.typescriptlang.org/docs/handbook/intro.html)
3. [MDN Web Docs - TypeScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/TypeScript)
4. [TypeScript Playground](https://www.typescriptlang.org/play)
5. [Introduction to TypeScript](https://www.tutorialspoint.com/typescript/typescript_introduction.htm)