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
### IF-ELSE:
```c
// C, C++, C#, Java, JavaScript, TypeScript, PHP, Kotlin

if (condicao1) {
  // code
} else if (condicao2) {
  // code
} else {
  // code
}
```
```python
# Python

if condicao1:
  // code
elif condicao2:
  // code
else:
  // code
// Python
```

### SWITCH (ou equivalente):
```c
// C, C++, C#, Java, JavaScript, TypeScript

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
}
```
```php
// PHP

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
}
```
```kotlin
// Kotlin

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
}
```
```python
# Python

if opcao == 1:
  // code
elif opcao == 2:
  // code
else:
  // code
```

## Declaração de Funções:
```c
// C, C++, C#, Java

int Soma(int x, int y) {
  return x + y;
}
```
```javascript
// JavaScript

function Soma(x, y) {
  return x + y;
}
```
```typescript
// TypeScript

function Soma(x: number, y: number): number {
  return x + y;
}
```
```php
// PHP

function Soma(int $x, int $y) {
  return $x + $y;
}
```
```kotlin
// Kotlin

fun Soma(x: Int, y: Int): Int {
  return x + y
}
```
```python
# Python

def Soma(x, y):
  return x + y
```