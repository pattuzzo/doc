# Comentários

## Sumário
- [O que são Comentários?](#o-que-são-comentários)
- [Comentários de Bloco](#comentários-inline)
- [Comentários de Bloco](#comentários-de-bloco)
- [Comentários de Documentação](#comentários-de-documentação)
- [Desativação de Código por Comentário](#desativação-de-código-por-comentário)
- [Referências](#referências)

## O que são Comentários?
Comentários são elementos essenciais na programação, proporcionando clareza e documentação para o código. Eles não afetam a execução do programa, mas desempenham um papel crucial na compreensão e manutenção do código fonte. Há dois tipos de comentários, inline e de bloco, e umas utilizações comuns, como comentários de documentação e de desativação de código.

## Comentários Inline
Os comentários inline são breves anotações incorporadas diretamente no código, geralmente após uma linha de código específica. Esses comentários fornecem insights rápidos sobre a funcionalidade ou intenção do código adjacente. São úteis para esclarecer partes específicas do código em que a intenção pode não ser imediatamente óbvia.

```javascript
let total = preco * quantidade; // Calcula o total baseado no preço e na quantidade.
```

## Comentários de Bloco
Comentários de bloco são ideais para anotações mais extensas que abrangem várias linhas de código. Eles são iniciados com `/*` e encerrados com `*/`. Esses comentários são valiosos para explicar o propósito de blocos de código, fornecendo uma visão abrangente de sua funcionalidade.

```javascript
/*
  Esta função realiza uma validação complexa,
  garantindo que os dados de entrada estejam
  corretos antes de continuar com o processamento.
*/
function validarDados() {
  // Implementação da validação...
}
```

## Comentários de Documentação
Comentários de documentação são especialmente importantes para gerar documentação automática do código. Eles seguem convenções específicas, como o formato JSDoc em JavaScript, e fornecem informações detalhadas sobre a função, seus parâmetros e o que ela retorna.

```javascript
/**
 * Calcula o quadrado de um número.
 * @param {number} x - O número para o qual calcular o quadrado.
 * @returns {number} - O quadrado do número fornecido.
 */
function calcularQuadrado(x) {
  return x * x;
}
```

## Desativação de Código por Comentário
Às vezes, é necessário desativar temporariamente um bloco de código para teste ou debug. Nesses casos, comentários podem ser usados para desativar seções de código, mantendo-as presentes para referência futura.

```javascript
/*
  if (condicao) {
    // Código a ser temporariamente desativado para teste.
    // ...
  }
*/
```

Ao incorporar essas práticas de comentários no código, os desenvolvedores contribuem significativamente para a compreensão e manutenção do software, facilitando a colaboração e o entendimento do código por outros membros da equipe.

## Referências
- **JavaScript.Info**:
  - [Comentários](https://javascript.info/structure#code-comments)
  - [Comentários Avançados](https://javascript.info/comments)
- **W3Schools**:
  - [Comentários](https://www.w3schools.com/js/js_comments.asp)