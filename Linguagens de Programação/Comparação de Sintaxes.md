# Comparação Entre Sintaxes

## Declaração de Variáveis:
```c
int quantidade = 5; // C, C++, C#, Java
let quantidade = 5; // JavaScript
let quantidade: number = 5; // TypeScript
$quantidade = 5; // PHP
var quantidade = 5 // Kotlin
quantidade = 5 // Python
```

## Tipos de Dados:
| Linguagem     | Tipos Inteiros               | Tipos de Ponto Flutuante  | Tipos Booleanos | Tipos Literais |     Outros      |
|---------------|------------------------------|---------------------------|------------------|---------------|-----------------|
| C             | int, short, long             | float, double             | _Bool            | char          |                 |
| C++           | int, short, long             | float, double             | bool             | char, string  |                 |
| C#            | int, short, long, byte       | float, double             | bool             | char, string  |                 |
| Java          | int, short, long, byte       | float, double             | boolean          | char, String  |                 |
| JavaScript    | number                       | number                    | boolean          | string        | null, undefined |
| TypeScript    | number                       | number                    | boolean          | string        | null, undefined |
| PHP           | int                          | float, double             | bool             | string        |                 |
| Kotlin        | Int, Short, Long, Byte       | Float, Double             | Boolean          | Char, String  |                 |
| Python        | int, complex                 | float                     | bool             | str           |                 |

## Estruturas Condicionais:
```c
if (condicao1) {
  // code
} else if (condicao2) {
  // code
} else {
  // code
} // C, C++, C#, Java, JavaScript, TypeScript, PHP, Kotlin

if condicao1:
  // code
elif condicao2:
  // code
else:
  // code
// Python


switch (opcao) {
  case 1:
    // code
    break;
  case 2:
    // code
    break;
  default:
    // code
    break;
} // C, C++, C#, Java, JavaScript, TypeScript

switch ($opcao) {
  case 1:
    // code
    break;
  case 2:
    // code
    break;
  default:
    // code
    break;
} // PHP

when (opcao) {
  1 -> {
    // code
  }
  2 -> {
    // code
  }
  else -> {
    // code
  }
} // Kotlin
```
```python
if opcao == 1:
  // code
elif opcao == 2:
  // code
else:
  // code
// Python
```

## Declaração de Funções:
```c
int Soma(int x, int y) {
  return x + y;
} // C, C++, C#, Java

function Soma(x, y) {
  return x + y;
} // JavaScript

function Soma(x: number, y: number): number {
  return x + y;
} // TypeScript

function Soma(int $x, int $y) {
  return $x + $y;
} // PHP

fun Soma(x: Int, y: Int): Int {
  return x + y
} // Kotlin

def Soma(x, y):
  return x + y
// Python
```