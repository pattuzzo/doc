# SolidJS

## Introdução ao SolidJS
Descrição
### JSX
Definição
Sintaxe
Explicação
### Componentes
Definição
Sintaxe
Funcionamento
### Props
Definição
Sintaxe
Funcionamento
### Renderização
Definição
Sintaxe
Funcionamento
Explicação

## JSX
Descrição
Sintaxe
Explicação
Definição
### Elementos JSX
Definição
Sintaxe
Explicação
Exemplo
Explicação
### Atributos JSX
Definição
Sintaxe
Explicação
Exemplo
Explicação
### Eventos JSX
Definição
Sintaxe
Explicação
Exemplo
Explicação
### Interpolação de Expressões JavaScript
Definição
Sintaxe
Explicação
Exemplo
Explicação

## Componentes
Descrição
Sintaxe
Parâmetros
### Props
Definição
Sintaxe
Explicação
### Retorno do Componente
Definição
Sintaxe
Explicação
### Instanciação de Componentes
Definição
Sintaxe
Explicação
Exemplo
Explicação
### Passagem de Props
Definição
Sintaxe
Explicação
Exemplo
Explicação
### Composição de Componentes
Definição
Sintaxe
Explicação
Exemplo
Explicação

## Props
Definição
Sintaxe
Explicação
Exemplo
Explicação
### Children
Definição
Sintaxe
Exemplo
Explicação
### Merge Props
Definição
Sintaxe
Parâmetros
Exemplo
Explicação
### Splitting Props
Definição
Sintaxe
Parâmetros
Exemplo
Explicação
### Desestruturação de Props
Descrição
Exemplo
Explicação
### Default Props
Descrição
Exemplo
Explicação

## Primitivos
Definição
### Signal
Descrição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
#### Signal Derivado
Definição
Exemplo
Explicação
### Effect
Descrição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### Memos
Descrição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação

## Store
Descrição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### Context
Descrição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
#### Produce

#### useContext
Descrição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação


## Controle de Fluxo
Descrição
### Show
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### Suspense
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### SuspenseList
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### Switch
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### Dynamic
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### For
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### Index
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### Portal
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### Error Boundary
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação

## Ciclo de Vida
Descrição
### onMount
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### onCleanup
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação
### onError
Definição
Sintaxe
Parâmetros
Funcionamento
Exemplo
Explicação

## Atributos JSX
### ref
Definição
Sintaxe
Explicação
### classList
Definição
Sintaxe
Explicação
### style
Definição
Sintaxe
Explicação













## Introdução ao SolidJS

O SolidJS é um framework JavaScript declarativo e reativo que proporciona um desempenho eficiente e uma experiência de desenvolvimento intuitiva. Neste tutorial, exploraremos os principais conceitos do SolidJS para ajudar você a criar aplicações modernas e reativas.

### JSX
JSX (JavaScript XML) é uma extensão de sintaxe do JavaScript que permite escrever código semelhante a XML/HTML. No SolidJS, JSX é utilizado para descrever a estrutura da interface do usuário.

##### Sintaxe
```jsx
function MinhaInterface() {
  return <div>Conteúdo JSX</div>;
}
```

O JSX simplifica a criação de elementos de interface, tornando o código mais legível e expressivo. O SolidJS compila o JSX para código JavaScript otimizado.

### Componentes
Os componentes no SolidJS são funções que aceitam um objeto de propriedades (`props`) e retornam elementos JSX. Eles são fundamentais para a estruturação e organização do código.

##### Sintaxe
```jsx
function MeuComponente(props) {
  return <div>{props.texto}</div>;
}
```

Os componentes são leves, sem estado próprio, e servem como fábricas de elementos JSX e primitivos reativos. Sua função é criar a visualização com base nas propriedades recebidas.

### Props
Props, ou propriedades, são objetos passados para os componentes e representam atributos vinculados ao JSX. No SolidJS, props são reativos e encapsulados em getters, garantindo consistência e reatividade.

##### Sintaxe
```jsx
<MeuComponente texto="Olá, SolidJS!" />
```

Os objetos props são somente leitura e mantêm a reatividade. Acessamos suas propriedades usando `.props.nomeDaPropriedade`. Evite desestruturação fora de um escopo de rastreamento para não perder a reatividade.

### Renderização
Renderização é o processo de transformar componentes e JSX em elementos visíveis na interface do usuário. No SolidJS, a renderização é eficiente e reativa.

##### Sintaxe
```jsx
import { render } from 'solid-js/web';

const App = () => <MinhaInterface />;
render(App, document.getElementById('app'));
```

A função `render` do SolidJS mapeia a hierarquia de componentes para o DOM, mantendo a sincronização reativa. Alterações nas propriedades ou estado dos componentes acionam automaticamente a atualização visual.

---

# JSX

O JSX, ou JavaScript XML, é uma extensão de sintaxe no JavaScript que facilita a construção de interfaces de usuário, especialmente em bibliotecas como React e SolidJS.
O JSX é uma sintaxe que permite a mistura de código JavaScript com marcação XML ou HTML. Ele simplifica a criação e atualização de elementos de interface de usuário.

##### Sintaxe
```javascript
const element = <h1>Hello, JSX!</h1>;
```
O JSX utiliza uma sintaxe semelhante ao XML ou HTML, permitindo a descrição de elementos de forma mais declarativa.
Durante a compilação, o JSX é transformado em chamadas de funções JavaScript. No caso do React, isso geralmente se traduz em chamadas para `React.createElement()`. Isso torna mais fácil criar hierarquias de elementos de maneira visualmente intuitiva.

### Elementos JSX
Os elementos JSX são a base da construção de interfaces de usuário. Eles representam a estrutura da UI e podem conter atributos, eventos e até mesmo outros elementos JSX.

##### Sintaxe
```javascript
const button = <button className="btn" onClick={handleClick}>Clique-me</button>;
```
Os elementos JSX podem conter atributos, como `className` para classes CSS e eventos, como `onClick` para lidar com interações do usuário. Eles podem ser aninhados para criar estruturas complexas.

### Atributos JSX
Os atributos JSX são usados para configurar propriedades e comportamentos dos elementos. Eles são semelhantes aos atributos HTML, mas permitem valores dinâmicos.

##### Sintaxe
```javascript
const input = <input type="text" value={inputValue} onChange={handleChange} />;
```
Os atributos JSX, como `value` e `onChange`, configuram propriedades do elemento. O uso de `{}` permite a inserção de valores dinâmicos, tornando a UI reativa às mudanças.

### Eventos JSX
Os eventos JSX permitem que você lide com interações do usuário, como cliques, teclas pressionadas, entre outros.

##### Sintaxe
```javascript
const handleClick = () => alert('Botão clicado!');
const button = <button onClick={handleClick}>Clique-me</button>;
```
Os eventos JSX, como `onClick`, são configurados para chamar funções JavaScript quando ocorrem interações do usuário. Isso proporciona uma maneira eficiente de tornar a UI interativa.

### Interpolação de Expressões JavaScript
A interpolação de expressões JavaScript no JSX permite incorporar dinamicamente valores e lógica de programação nas marcações.

##### Sintaxe
```javascript
const name = 'SolidJS';
const greeting = <p>Hello, {name}!</p>;
```
Ao usar `{}`, é possível incorporar expressões JavaScript diretamente no JSX. Isso é fundamental para criar interfaces dinâmicas que respondem a variáveis e dados em tempo real.

Este conjunto de tópicos abrange desde a definição até exemplos práticos de como usar elementos, atributos, eventos e interpolação de expressões JavaScript no JSX. Esses conceitos são fundamentais para desenvolvedores que desejam criar interfaces de usuário reativas e eficientes com JSX em projetos JavaScript.

---

## Componentes

Os componentes são blocos fundamentais no desenvolvimento de interfaces de usuário modulares e reutilizáveis em frameworks como React e SolidJS. Eles representam unidades independentes de funcionalidade e interface, encapsulando lógica, estilo e marcação, proporcionando uma abordagem estruturada para construir aplicações.

Os componentes são como peças autossuficientes que, quando combinadas, formam a estrutura de uma aplicação. Eles podem ser compostos por elementos JSX, lógica, estilos e outros componentes. Essa modularidade facilita a manutenção, teste e reutilização de código, uma vez que diferentes partes da interface são encapsuladas e isoladas umas das outras.

##### Sintaxe
```javascript
// Exemplo de componente em SolidJS
const MyComponent = (props) => {
  // Corpo do componente
};
```

##### Parâmetros
- `props`: Objeto que contém propriedades passadas ao componente. São utilizadas para transmitir dados ao componente e podem ser acessadas como propriedades do objeto `props`.

### Props
Props, abreviação de propriedades, referem-se aos dados que são passados para um componente. Essas propriedades são utilizadas para configurar e personalizar a funcionalidade e a aparência do componente.

##### Sintaxe
```javascript
// Exemplo de componente com props em SolidJS
const Greeting = (props) => {
  // Corpo do componente usando props
};
```

No exemplo acima, o componente `Greeting` recebe propriedades por meio do objeto `props`. Essas propriedades podem ser acessadas dentro do componente, permitindo a personalização dinâmica da saudação exibida.

### Retorno do Componente
O retorno do componente refere-se ao que um componente renderiza na interface do usuário. Em frameworks como SolidJS, um componente pode retornar apenas um elemento JSX diretamente, mas pode encapsular múltiplos elementos em uma estrutura, como um fragmento.

##### Sintaxe
```javascript
// Exemplo de retorno de componente em SolidJS
const HelloWorld = () => {
  return <div>Hello, World!</div>;
};
```

Em SolidJS, um componente pode encapsular vários elementos em um fragmento ou diretamente retornar um único elemento JSX. A escolha depende da estrutura desejada e da necessidade de um envoltório adicional.

### Instanciação de Componentes

A instanciação de componentes refere-se ao processo de criar e utilizar uma instância específica de um componente em um aplicativo. Isso envolve a chamada de um componente como se fosse um elemento para gerar uma representação específica desse componente na interface do usuário.

##### Sintaxe
```javascript
// Exemplo de declaração de componente em SolidJS
const MyComponent = (props) => {
  return <div>{props.message}</div>;
};

// Exemplo de instanciação de componente em SolidJS
const App = () => {
  return (
    <div>
      <MyComponent message="Hello, SolidJS!" />
    </div>
  );
};
```

No exemplo acima, `MyComponent` está sendo instanciado como um elemento dentro do componente `App`. Isso cria uma instância específica de `MyComponent`, incorporando-o à estrutura da interface do usuário.

##### Exemplo
```javascript
// Outro exemplo de instanciação de componente em SolidJS
const ParentComponent = () => {
  return (
    <div>
      <ChildComponent />
      <ChildComponent />
    </div>
  );
};
```

Aqui, `ChildComponent` está sendo instanciado duas vezes dentro de `ParentComponent`, demonstrando a capacidade de reutilização e composição de componentes.

### Passagem de Props

A passagem de props é o mecanismo pelo qual dados são transmitidos de um componente pai para um componente filho. Isso permite a personalização e configuração dinâmica dos componentes com base nas necessidades específicas do aplicativo.

##### Sintaxe
```javascript
// Exemplo de declaração de componente em SolidJS
const Greeting = (props) => {
  return <div>{props.message}</div>;
};

// Exemplo de passagem de props em SolidJS
const App = () => {
  const message = "Hello, SolidJS!";
  return (
    <div>
      <Greeting message={message} />
    </div>
  );
};
```

No exemplo acima, a propriedade `message` é passada para o componente `Greeting` como parte da instância desse componente. Isso permite que o componente filho utilize dinamicamente a mensagem recebida.

##### Exemplo
```javascript
// Outro exemplo de passagem de props em SolidJS
const ParentComponent = () => {
  return (
    <div>
      <ChildComponent name="John" age={25} />
    </div>
  );
};
```

Aqui, `ParentComponent` está passando as props `name` e `age` para `ChildComponent`. Essas props podem ser acessadas dentro de `ChildComponent` para personalizar seu comportamento.

### Composição de Componentes

A composição de componentes refere-se à prática de combinar e utilizar vários componentes para construir interfaces de usuário mais complexas. Isso permite a criação de interfaces modulares e a reutilização eficiente de código.

##### Sintaxe
```javascript
// Exemplo de declaração de componentes em SolidJS
const Header = () => {
  return <div>Header Component</div>;
};

const MainContent = () => {
  return <div>Main Content Component</div>;
};

const Footer = () => {
  return <div>Footer Component</div>;
};

// Exemplo de composição de componentes em SolidJS
const App = () => {
  return (
    <div>
      <Header />
      <MainContent />
      <Footer />
    </div>
  );
};
```

No exemplo acima, `App` está compondo a interface do usuário combinando os componentes `Header`, `MainContent`, e `Footer`. Isso facilita a organização e manutenção do código.

##### Exemplo
```javascript
// Outro exemplo de composição de componentes em SolidJS
const BlogPost = () => {
  return (
    <div>
      <PostHeader />
      <PostContent />
      <PostComments />
    </div>
  );
};
```

Aqui, `BlogPost` está compondo uma postagem de blog combinando os componentes `PostHeader`, `PostContent`, e `PostComments`. Isso ilustra como a composição de componentes permite a construção de interfaces mais sofisticadas a partir de partes reutilizáveis.

---

## Props

Props, abreviação de propriedades, no contexto do SolidJS, são objetos que são passados para a função do componente durante a execução. Esses objetos representam todos os atributos vinculados ao componente na sua instanciação e são somente leitura. Eles contêm propriedades reativas encapsuladas em getters de objeto, proporcionando uma forma consistente independentemente do uso de sinais, expressões de sinal ou valores estáticos.

##### Sintaxe
```jsx
function MyComponent(props) {
  // Corpo do componente
};

<MyComponent prop1={value1} prop2={value2} />
```

Props são utilizados para permitir a comunicação entre componentes no SolidJS, sendo uma maneira eficiente de passar dados de um componente pai para um componente filho. Eles são acessados por meio da notação `props.propName`. Vale ressaltar que Props são objetos somente leitura, garantindo integridade durante a renderização e re-renderização dos componentes.

##### Exemplo
```jsx
// Exemplo de componente utilizando Props em SolidJS
function Greeting(props) {
  return <div>Hello, {props.name}!</div>;
};

<Greeting name="John" />
```

No exemplo acima, o componente `Greeting` recebe a propriedade `name` por meio do objeto `props`. Essa propriedade é acessada dentro do componente para personalizar dinamicamente a saudação exibida. Props oferecem uma forma flexível de configurar e adaptar componentes em aplicações SolidJS.

### Children

No SolidJS, a propriedade `children` refere-se ao conteúdo incluído entre as tags de abertura e fechamento de um componente. É uma propriedade especial que contém os elementos ou texto passados como filhos do componente.

##### Sintaxe
```jsx
<MyComponent>
  Conteúdo como Children
</MyComponent>
```

##### Exemplo
```jsx
// ParentComponent.tsx
export default function ParentComponent(props) {
  return <div>{props.children}</div>;
}

// App.tsx
import ParentComponent from './ParentComponent';

function App() {
  return (
    <ParentComponent>
      Conteúdo Renderizado como Children
    </ParentComponent>
  );
}
```

No exemplo acima, `ParentComponent` possui a propriedade `children`, que é onde o conteúdo entre as tags de abertura e fechamento é renderizado. Isso permite a criação de componentes mais flexíveis que podem envolver e renderizar dinamicamente o conteúdo fornecido como filhos.

### Default Props

No SolidJS, o uso de valores padrão diretamente na desestruturação de `props` pode levar a problemas de reatividade. Quando você define um valor padrão usando a lógica tradicional de desestruturação, esse valor é resolvido durante a criação do componente e não é reavaliado quando os `props` mudam. Isso pode resultar em comportamentos inesperados, especialmente ao lidar com valores reativos.

##### Exemplo
```jsx
const BasicComponent = (props) => {
  const value = props.value || "default";

  return <div>{value}</div>;
};
```

No exemplo acima, o valor padrão para `value` é definido usando a lógica tradicional de desestruturação. Isso significa que, durante a criação do componente, `value` é resolvido e não é atualizado automaticamente quando os `props` mudam. Isso pode levar a resultados inesperados, já que `value` permanecerá como "default" mesmo se `props.value` for alterado.

#### Alternativas

##### Acessar `props` diretamente no JSX

```jsx
const BasicComponent = (props) => {
  return <div>{props.value || "default"}</div>;
};
```

Nesta alternativa, a lógica para fornecer um valor padrão é incorporada diretamente no JSX, utilizando a expressão lógica `props.value || "default"`. Isso permite acessar `props` diretamente e renderizar o valor de `props.value`, ou o valor padrão "default" se `props.value` for falsy. Essa abordagem é simples e adequada para casos em que a lógica é direta e não envolve cálculos complexos.

##### Içar a Lógica para uma Função

```jsx
const BasicComponent = (props) => {
  const value = () => props.value || "default";

  return <div>{value()}</div>;
};
```

Nesta abordagem, a lógica para fornecer um valor padrão é içada para uma função chamada `value`. A função é então invocada no JSX para obter o valor a ser renderizado. Içar a lógica para uma função permite reutilização e clareza, mantendo a reatividade ao acessar `props.value`. No entanto, a função `value` precisa ser invocada para obter o valor atualizado.

##### Utilizar `createMemo` para Cálculos Custosos

```jsx
import { createMemo } from "solid-js";

const BasicComponent = (props) => {
  const value = createMemo(() => props.value || "default");

  return <div>{value()}</div>;
};
```

Nesta alternativa, `createMemo` é utilizado para criar uma memoização do cálculo do valor padrão. Isso é útil quando a lógica de cálculo é mais custosa e não precisa ser recalculada a cada renderização. `createMemo` garante que o valor seja recalculado apenas quando as dependências, neste caso `props.value`, são alteradas. Isso proporciona uma otimização em termos de desempenho.

##### Usar `mergeProps` como Helper

```jsx
import { mergeProps } from "solid-js";

const BasicComponent = (props) => {
  props = mergeProps({ value: "default" }, props);

  return <div>{props.value}</div>;
};
```

Nesta alternativa, `mergeProps` é utilizado como um helper para mesclar um objeto padrão contendo a propriedade `value` com o objeto `props`. Isso garante que `props.value` seja reativo e, ao mesmo tempo, fornece um valor padrão quando necessário. Utilizar `mergeProps` simplifica a lógica e mantém a reatividade, sendo uma escolha eficaz para cenários que envolvem valores padrão em objetos de `props`.

## Merge Props
`mergeProps` é uma utilidade do SolidJS que mescla objetos potencialmente reativos, de forma não destrutiva, sem perder a reatividade. Essa função é útil para definir adereços padrão para componentes, garantindo que as atualizações reativas sejam preservadas.

### Sintaxe
```jsx
const mergedProps = mergeProps({ key1: value1, key2: value2 }, props);
```

### Parâmetros
- `{ key1: value1, key2: value2 }`: Lista de pares chave-valor que representa as propriedades padrão.
- `props`: O objeto props do componente.

### Exemplo
```jsx
// greetings.tsx
import { mergeProps } from 'solid-js/web';

export default function Greeting(props) {
  const merged = mergeProps({ greeting: "Hi", name: "John" }, props);
  return <h3>{merged.greeting} {merged.name}</h3>
}
```
No exemplo acima, `mergeProps` é usado para mesclar objetos padrão e objetos de adereços, garantindo que as propriedades reativas sejam preservadas. Isso é útil ao definir padrões para componentes sem perder a reatividade nas atualizações.

### Desestruturação de Props em SolidJS
Em SolidJS, a desestruturação direta de Props não é uma prática recomendada, pois pode resultar na perda de reatividade. A reatividade é um aspecto crucial do SolidJS, e acessar propriedades diretamente por meio da desestruturação pode quebrar esse vínculo dinâmico.

##### Exemplo
```jsx
// GreetingComponent.tsx
export default function GreetingComponent(props) {
  const { name, message } = props;
  return <div>{message}, {name}!</div>;
}

// App.tsx
import GreetingComponent from './GreetingComponent';

function App() {
  return <GreetingComponent name="John" message="Hello" />;
}
```

No exemplo acima, a desestruturação direta de `props` é usada para extrair as propriedades `name` e `message`. No entanto, essa abordagem pode levar à perda de reatividade, pois o SolidJS não consegue rastrear as propriedades individualmente quando desestruturadas.

#### Alternativa `splitProps`

Em vez de desestruturar diretamente, é recomendável usar a função `splitProps` para dividir as propriedades, mantendo a reatividade:

```jsx
// GreetingComponent.tsx
import { splitProps } from 'solid-js/web';

export default function GreetingComponent(props) {
  const [localProps] = splitProps(props, ['name', 'message']);
  return <div>{localProps.message}, {localProps.name}!</div>;
}

// App.tsx
import GreetingComponent from './GreetingComponent';

function App() {
  return <GreetingComponent name="John" message="Hello" />;
}
```

Ao usar `splitProps`, as propriedades são mantidas como reativas, garantindo que qualquer atualização nos dados seja refletida corretamente na renderização do componente.

## Splitting Props
`splitProps` é uma utilidade do SolidJS que divide o objeto `props` em grupos, permitindo a extração de algumas propriedades para utilização no componente atual e outras para passar para componentes filhos. Ele preserva a reatividade em todos os objetos resultantes.

### Sintaxe
```jsx
const [localProps, others] = splitProps(props, ['prop1', 'prop2']);
```

### Parâmetros
- `props`: O objeto de adereços a ser dividido.
- `['prop1', 'prop2', ...]`: Matrizes de chaves que indicam quais propriedades extrair para objetos separados.

### Exemplo
```jsx
// greeting.tsx
import { splitProps } from 'solid-js/web';

export default function Greeting(props) {
  const [local, others] = splitProps(props, ["greeting", "name"]);
  return <h3 {...others}>{local.greeting} {local.name}</h3>
}
```
No exemplo acima, `splitProps` é usado para dividir o objeto `props` em duas partes: `local` contendo as propriedades específicas para o componente atual e `others` contendo as propriedades restantes para passar para componentes filhos. Essa abordagem preserva a reatividade em ambos os conjuntos de propriedades resultantes.

---

### Primitivos

No contexto do SolidJS, os primitivos referem-se às entidades fundamentais que constituem a base da biblioteca. Esses primitivos são essenciais para o paradigma reativo do SolidJS, proporcionando um modelo de programação reativa eficiente. Os principais primitivos incluem Signals, Effects e Memos.

Os primitivos do SolidJS são:

1. **Signal:** Representa um valor que pode ser observado. Quando um Signal é atualizado, os componentes dependentes são automaticamente notificados para reavaliação.

2. **Effect:** É uma função que reage a mudanças em Signals. É utilizado para realizar efeitos colaterais, como ações assíncronas ou atualizações de interface do usuário.

3. **Memo:** Armazena valores derivados com base em Signals e Effects, oferecendo uma maneira eficiente de calcular e armazenar resultados complexos apenas quando necessário.

Esses primitivos formam o cerne da programação reativa no SolidJS, permitindo o desenvolvimento de interfaces de usuário dinâmicas e responsivas.

Observação: O entendimento e uso adequado desses primitivos são fundamentais para tirar o máximo proveito da abordagem reativa do SolidJS.

### Signal

Signal é uma primitiva fundamental no Solid que atua como um emissor de eventos, contendo um valor e funções get e set para interceptar leituras e escritas. Ele desempenha um papel crucial no rastreamento automático de dependências e na reatividade do Solid.

##### Sintaxe
```javascript
const [count, setCount] = createSignal(0);
```

##### Parâmetros
- `initialValue`: O valor inicial do Signal.

Os Signals notificam automaticamente seus assinantes sempre que seu valor é modificado. Eles são a base para o rastreamento de dependências e a execução de Effects e Memos.

##### Exemplo
```javascript
// Em um componente Solid
const Counter = () => {
  const [count, setCount] = createSignal(0);

  return (
    <div>
      <p>Contagem: {count()}</p>
      <button onClick={() => setCount(count() + 1)}>Incrementar</button>
    </div>
  );
};
```

No exemplo, `count` é um Signal com valor inicial de 0. O componente `Counter` usa o Signal para rastrear e exibir a contagem. Quando o botão é clicado, `setCount` é chamado, atualizando o valor de `count` e, assim, reativamente atualizando a exibição da contagem.

#### Signal Derivado

Signal Derivado é um Signal que depende de um ou mais Signals existentes, sendo atualizado sempre que seus Signals de origem são modificados.

##### Exemplo
```javascript
// Em um componente Solid
const CounterWithDerived = () => {
  const [count, setCount] = createSignal(0);
  const doubledCount = () => count() * 2;

  return (
    <div>
      <p>Contagem: {count()}</p>
      <p>Contagem Duplicada: {doubledCount()}</p>
      <button onClick={() => setCount(count() + 1)}>Incrementar</button>
    </div>
  );
};
```

`doubledCount` é um Signal Derivado que depende do Signal `count`. Sempre que `count` é modificado, `doubledCount` é recalculado automaticamente, mantendo-se sincronizado com seu(s) Signal(is) de origem. O componente `CounterWithDerived` exibe tanto a contagem quanto a contagem duplicada, ambas reativamente atualizadas.

### Effect

Effect é uma primitiva no Solid usada para criar efeitos colaterais ou executar ações secundárias em resposta a mudanças em Signals dependentes. Ele desempenha um papel crucial na criação de lógicas reativas e na gestão de efeitos em um aplicativo Solid.

##### Sintaxe
```javascript
createEffect(() => {
  // Lógica do efeito
});
```

##### Parâmetros
- `effectFunction`: Uma função contendo a lógica do efeito.

Effects são executados automaticamente sempre que Signals dependentes são modificados. Eles proporcionam uma maneira estruturada de lidar com efeitos colaterais, como manipulação do DOM, chamadas de API, etc.

##### Exemplo
```javascript
// Em um componente Solid
const LoggerComponent = () => {
  const [message, setMessage] = createSignal("");

  createEffect(() => {
    console.log("Mensagem atual:", message());
  });

  return (
    <div>
      <input type="text" value={message()} onInput={(e) => setMessage(e.target.value)} />
    </div>
  );
};
```

Neste exemplo, `LoggerComponent` cria um Effect que loga a mensagem atual sempre que ela é modificada. O efeito é acionado automaticamente quando o usuário digita no campo de entrada, proporcionando um mecanismo reativo para a ação de log.

Observação: Effects podem ter dependências explícitas, o que significa que só serão executados quando os Signals específicos forem modificados.

Essa estrutura ajuda a manter a coesão e facilita a compreensão da lógica reativa no código Solid.

### Memos

Memos são primitivas fundamentais no Solid que oferecem a capacidade de armazenar valores derivados com base em Signals e Effects. Eles proporcionam uma maneira eficiente de realizar cálculos computacionais complexos apenas quando necessário, evitando repetições desnecessárias.

##### Sintaxe
```javascript
const factorialMemo = createMemo(() => factorial(count()));
```

##### Parâmetros
- `memoFunction`: Uma função contendo a lógica para calcular o valor do Memo.

Memos armazenam em cache o resultado da execução da função fornecida como argumento. Eles são reavaliados automaticamente apenas quando as Signals referenciadas na função são modificadas.

##### Exemplo Sem Memo
```javascript
// Em um componente Solid
const MemoComponentWithoutMemo = () => {
  const [count, setCount] = createSignal(1);

  const factorial = (n) => {
    if (n === 0 || n === 1) return 1;
    return n * factorial(n - 1);
  };

  const factorialWithoutMemo = () => factorial(count());

  return (
    <div>
      <button onClick={() => setCount(count() + 1)}>Incrementar Contador</button>
      <div>
        <p>1. {factorialWithoutMemo()} {factorialWithoutMemo()} {factorialWithoutMemo()} {factorialWithoutMemo()} {factorialWithoutMemo()}</p>
      </div>
    </div>
  );
};
```

##### Exemplo Com Memo
```javascript
// Em um componente Solid
const MemoComponentWithMemo = () => {
  const [count, setCount] = createSignal(1);

  const factorial = (n) => {
    if (n === 0 || n === 1) return 1;
    return n * factorial(n - 1);
  };

  const factorialMemo = createMemo(() => factorial(count()));

  return (
    <div>
      <button onClick={() => setCount(count() + 1)}>Incrementar Contador</button>
      <div>
        <p>1. {factorialMemo()} {factorialMemo()} {factorialMemo()} {factorialMemo()} {factorialMemo()}</p>
      </div>
    </div>
  );
};
```

Os exemplos demonstram a diferença de desempenho entre calcular o fatorial sem Memo e com Memo. O exemplo sem Memo chama repetidamente a função `factorial`, resultando em uma performance inferior. Com Memo, o valor é armazenado em cache, evitando cálculos redundantes e otimizando a eficiência do componente. O Memo garante que a função seja reavaliada apenas quando necessário, melhorando a performance da aplicação.