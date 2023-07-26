
Definição
=========

Segundo Schildt (1996), ponteiro é uma variável que contém um endereço de memória. Podemos ainda definir o ponteiro como um tipo especial de variável, na qual o valor atribuído é um endereço de memória.

Ou seja, ponteiro ou apontador é uma variável capaz de armazenar um endereço de memória ou o endereço de outra variável.

Para entendermos melhor essa definição, precisamos compreender como a memória de um programa é organizada e o que é um endereço de memória.

Memória
=======

Memória é um componente do computador responsável pelo armazenamento de dados e instruções. Ela é composta por palavras, sendo cada palavra identificada unicamente a partir de um endereço, ou seja, um endereço de memória.

Cada palavra tem uma capacidade de armazenamento da informação, isto é, uma quantidade de bytes que a palavra representa.

Sendo assim, aprendemos que uma memória é composta por palavras e que toda palavra possui um endereço único, conforme é visto na Tabela 1.

Endereço

Palavras

0 (00)

Palavra 0

1 (001)

Palavra 1

2 (010)

Palavra 2

3 (011)

Palavra 3

4 (100)

Palavra 4

5 (101)

Palavra 5

6 (110)

Palavra 6

Tabela 1: Representação da memória. Fonte: O Autor.

__ **Atenção!** Para visualização completa da tabela utilize a rolagem horizontal

O endereço de memória de um processo em execução é dividido em vários segmentos lógicos. Destacamos alguns dos mais importantes:

Clique nas barras para ver as informações. Objeto com interação.

Text
====

Contém o código do programa e suas constantes. Este segmento é alocado durante a criação do processo (''exec'') e permanece do mesmo tamanho durante toda a vida do processo.

Data
====

Este segmento é a memória de trabalho do processo, na qual ficam alocadas as variáveis globais e estáticas. Tem tamanho fixo ao longo da execução do processo.

Stack
=====

Contém a pilha de execução, na qual são armazenados os parâmetros, endereços de retorno e variáveis locais de funções. Pode variar de tamanho durante a execução do processo.

Heap
====

Contém blocos de memória alocadas dinamicamente, a pedido do processo, durante sua execução. Varia de tamanho durante a vida do processo.

Podemos observar na Figura 1 a distribuição dos segmentos lógicos do endereço de memória.

![](img/img_01.jpg " Fonte:O Autor")

Figura 1: Seguimentos lógicos do endereço de memória. Fonte: O Autor.

												
`1 	#include < stdio.h >  2	 3 	static int a = 0;  // variável global, alocação estática 4 5 	void incrementa(void) 6 	{ 7 		int b = 0; // variável local, alocação automática 8 		static int c = 0; // variável local, alocação estática 9  10 		printf ("a: %d, b: %d, c: %d\n", a, b, c); 11		a++; 12 		b++; 13 		c++; 14 	} 15 16 	int main(void) 17 	{ 18		int i; 19		for (i = 0; i < 5; i++) 20		incrementa(); 21 		system("pause"); 22 		return(0); 23	}`													
												
											

Exemplo 1: Alocação de memória. Fonte: O Autor.

### **Comentário**

Voltando a observar o Exemplo 1, a variável “b” é declarada de forma automática ao ser invocada a função incrementa, conforme a linha 7 do código-fonte, e descartada quando a função se encerra.

`#include < stdlib.h >`  
`void free (void *ptr)`  

`#include < stdlib.h >`  
`void * realloc (void *ptr, size_t newsize)`  

`#include < stdlib.h >`  
`void * calloc (size_t count, size_t eltSize)`  

`int x = 5;`  
`char c = ’D’;`  

![](img/img_04.jpg "Fonte:Shutterstock")

Figura 4: Ponteiro armazena endereço da variável “x”. Fonte: O Autor.

A figura 4 apresenta uma memória que armazena a variável “x” e o ponteiro para a variável “x”. Como o conteúdo do ponteiro é um endereço, a seta indica a relação entre o ponteiro e a variável que ele aponta.

Tipo\_da\_variável \* Nome\_da\_Variável;

pt\_x = &x;

\*pt\_x = 50;

/\* 4 x sizeof(int) = 16 bytes \*/

pt = pt + 4;

__ **Atenção!** Para visualização completa da equação utilize a rolagem horizontal

`//atribuindo o endereço de v_num ao ponteiro`  
`ptr = &v_num;`  

EMPREGANDO PONTEIROS E ALOCAÇÃO DINÂMICA
========================================

  ![](./img/imagem_full2.jpg "Fonte: Shutterstock")

Tipos de estrutura de dados
===========================

Uma estrutura de dados pode ser dividida em: **Dado e estrutura**.

O **dado** é o elemento que possui valor agregado e que pode ser utilizado para solucionar problemas computacionais. Os dados possuem tipos específicos. Por padrão, são quatro tipos de dados.

Inteiro

Representa valores numéricos negativos ou positivos sem casa decimal, ou seja, valores inteiros.

Real

Representa valores numéricos negativos ou positivos com casa decimal, ou seja, valores reais. Também são chamados de ponto flutuante.

Lógico

Representa valores booleanos, assumindo apenas dois estados, verdadeiro ou falso. Pode ser representado apenas um bit (que aceita apenas 1 ou 0).

Texto

Representa uma sequência de um ou mais caracteres, colocamos os valores do tipo texto entre “” (aspa duplas).

__ **Atenção!** Para visualização completa da tabela utilize a rolagem horizontal

O tipo de dados texto pode ser subdividido em string ou caractere, e o tipo de dado real em ponto flutuante com precisão simples (float) ou ponto flutuante com precisão dupla (double).

A estrutura é o elemento responsável por carregar as informações dentro de uma estrutura de software. Alguns tipos de estrutura são: Vetores multidimensionais, pilhas, filas, listas, árvores, grafos, tabelas hashing, dentre outros.

Vamos conhecer os principais tipos de estrutura de dados citados anteriormente.

Clique nas palavras. Objeto com interação.

[Vetores unidimensionais e bidimensionais](javascript:void(0))

[Fila](javascript:void(0))

[Árvore](javascript:void(0))

[Lista encadeada](javascript:void(0))

[Pilha](javascript:void(0))

[Grafo](javascript:void(0))

__ **Atenção!** Para visualizaçãocompleta da tabela utilize a rolagem horizontal

Nas estruturas de dados homogêneas, a individualização de cada variável é feita através do uso de índices. No caso dos vetores que são matrizes de uma só dimensão, é necessário apenas 1 índice para acesso às variáveis.

![](img/img_12.jpg "Fonte: O Autor")

Figura 11: Exemplo de vetor. Fonte: O Autor.

Registro Funcionário

Matrícula

Tipo Inteiro

Nome

Tipo Cadeia de Caracteres

Dt. Nascimento

Tipo Data

Cargo

Tipo Cadeia de Caracteres

Salário

Tipo Real

__ **Atenção!** Para visualização completa da tabela utilize a rolagem horizontal

    
    var Ficha_Funcionario: registro
    inicio
    	matricula: inteiro
    	nome: vetor[1..50] de caractere
    	Dt_Nascimento: vetor[1..9] de caractere
    	Cargo: vetor[1..30] de caractere
    	Salario: real
    fim
    

leia(Ficha\_Funcionario.matricula)

escreva(Ficha\_Funcionario.nome)

Ficha\_Funcionario.**_cargo_** <- “gerente”

Matrícula

Nome

D. Nascimento

Cargo

Salário

Tabela 4 : Exemplo da Tabela de Registro de Funcionário.

__ **Atenção!** Para visualização completa da tabela utilize a rolagem horizontal

Definição de struct em C
========================

Na linguagem C, existem dois tipos de dados: Os tipos básicos (int, char, float, double, void) e os tipos compostos homogêneos (arrays). Porém, nem sempre estes tipos são suficientes para o programa e, por isso, a linguagem C nos permite a criação de outras estruturas de dados, a partir dos tipos básicos, como os registros.

Na linguagem C, os registros são representados com uma estrutura denominada struct, que é uma coleção de variáveis relacionadas, usando um nome comum. As estruturas de dados em linguagem C podem conter variáveis de tipos diferentes de dados, ao contrário de um array, que só pode conter dados de um mesmo tipo.

### **Você sabia**

As estruturas (struct) são usadas para definir registros que são armazenados em arquivos e, com os ponteiros, simplificam a criação de estruturas de dados mais complexas, por exemplo, pilhas, listas ligadas, filas e árvores.

Sendo assim, entendemos que as estruturas são um tipo de dados derivado, o que significa que são construídas com o uso de objetos de outros tipos existentes.

Definimos um modelo de estrutura na linguagem C como mostrado na figura.

												
`struct identificador {   	tipo variável; tipo variável; 	tipo variável;  	tipo variável; };`
												  
												
											

Em resumo, struct é um conjunto de variáveis sob o mesmo nome, e definido pelo programador. E cada variável dentro de uma estrutura pode ser de um tipo diferente, ou melhor, não é obrigatório que sejam todas do mesmo tipo.

Visualizamos, logo abaixo, um exemplo de definição de struct. A palavra-chave struct inicia o bloco de definição da estrutura. Logo após, vem o nome que desejamos atribuir à estrutura (tag da estrutura), e então são abertas chaves “**{**“ para iniciar a seção do corpo da estrutura.

												
`struct mystruct {    char a;    int b;    flaot c; };`
											

Neste outro exemplo, é possível visualizar a definição de uma estrutura de nome endereço, contendo os membros rua, número, CEP e bairro:

												
`struct endereco {  	char rua[50]; 	char numero[5]; 	char CEP[8]; 	char bairro[30]; };`
											

												
`struct nome_da_estrutura {  	tipo_campo1  nome_campo1; 	tipo_campo2  nome_campo2;  	...  } variáveis_que_armazenam_a_estrutura;` 
										
											

												
`struct livro { 	char nome[30]; 	char autor[50]; 	int paginas; 	float preco; } livro1, livro2, livro3;`
											

Inicializando struct em C
=========================

A estrutura de dados struct em linguagem C possui uma inicialização parecida com os vetores e as matrizes.

Uma das maneiras de inicializar uma struct é através de uma lista de inicialização, como um array. Agora, se o número de inicializadores na lista for menor que os membros na estrutura, os membros restantes serão automaticamente inicializados em zero ou Null, se o membro for um ponteiro.

Por exemplo, podemos inicializar a estrutura endereço usando a declaração a seguir. Observe que os elementos do array são passados aos membros da estrutura na ordem em que foram declarados.

`struct endereco x = {"Av. das Américas", "4200", " 22640-102 ", "Barra da Tijuca"};`  

Outra forma é atribuindo uma variável estrutura do mesmo tipo, já inicializada.

Por último, atribuindo valores aos membros individuais da estrutura. Por exemplo, suponha que desejamos atribuir o valor “Av. das Américas” ao membro rua da estrutura endereco.

Podemos usar a declaração a seguir, referenciando o nome da variável estrutura, seguida por um ponto e pelo nome do membro (campo) que receberá a atribuição do dado.

endereco.rua = "Av. das Américas";

printf("%s", x.rua);

Manipulando structs
===================

As estruturas de dados structs podem ser manipuladas com o objetivo de acessar os campos, atribuir valores para os campos, imprimir os valores dos campos, dentre outros.

Para atribuir valores aos campos da estrutura, você faz isto diretamente, e em qualquer parte do programa, conforme a seguir:

												
`aluno_especial.codigo = 10; strcpy(aluno_especial.nome, "Manoel"); aluno_especial.nota = 10.0;`
											

Para atribuir um valor a uma string, é necessário utilizar a função strcpy (CPY = copiar; STR = string). A função copiará o que está dentro das aspas duplas para o campo STRING da estrutura.

É possível imprimir os valores dos campos da estrutura em qualquer parte do programa utilizando a função printf.

												
`printf(" \n %d ", aluno_especial.codigo); printf(" \n %s ", aluno_especial.nome); printf(" \n %.2f ", aluno_especial.nota);`
											

Entretanto, se for preciso imprimir todos os membros da estrutura de uma única vez, é recomendável criar uma função para isto.

												
`void imprimir(Aluno aluno_regular){ 	printf(" \n %d ", aluno_especial.codigo);  	printf(" \n %s ", aluno_especial.nome);  	printf(" \n %.2f ", aluno_especial.nota); }`
											

Observe que a função de impressão é do tipo Void, mas tem um argumento, isto é, é definida uma variável do tipo da estrutura, significando que, ao chamar a função, você deverá passar como parâmetro a estrutura que está trabalhando.

A chamada fica da seguinte forma:

imprimir(aluno\_especial);

Para obter dados do teclado, devemos utilizar a função scanf, como em outras situações para entrada de dados na linguagem C. Podemos obter dados do teclado em qualquer parte do programa, assim como também podemos definir uma função para realizar este trabalho.

												
`printf(" Digite o código do aluno especial: "); scanf("%d%*c", &aluno_especial.codigo); printf(" Digite o nome do aluno especial: "); scanf("%s%*c", &aluno_especial.nome); printf(" Digite a nota do aluno especial: "); scanf("%f%*c", &aluno_especial.nota);`
											

												
`void cadastrar(Aluno aluno_especial){ 	printf(" Digite o código do aluno especial: ");  	scanf("%d%*c", &aluno_especial.codigo);  	printf(" Digite o nome do aluno especial: ");  	scanf("%s%*c", &aluno_especial.nome);  	printf(" Digite a nota do aluno especial: ");  	scanf("%f%*c", &aluno_especial.nota); }`
											

Observe que na função cadastrar e imprimir é passado como parâmetro (por valor) a variável do tipo estrutura. Em algumas ocasiões, você precisará fazer desta forma, em outras, talvez você não tenha que passar a estrutura como parâmetro.

### Exemplos práticos

No Exemplo 5, vamos criar uma struct para armazenar os dados do aluno.

Exemplo 5:

1`/* Cria uma estrutura para armazenar dados de um aluno*/`  
2`#include < stdio.h >`  
3 `#include < stdlib.h >`  
4  
5 `struct aluno {`  
6`int v_nmat; //número da matrícula`  
7`float v_nota[3]; //notas`  
8`float v_media; //media`  
9`};`  
10  
11`int main() {`  
12`struct aluno Felipe; //declara uma variável do tipo struct`  
13`Felipe.v_nmat = 120;`  
14`Felipe.v_nota[0]=8.5;`  
15`Felipe.v_nota[1]=7.2;`  
16`Felipe.v_nota[2]=5.4;`  
17`Felipe.v_media=(Felipe.v_nota[0]+ Felipe.v_nota[1]+ Felipe.v_nota[2])/3.0;`  
18`printf(“Matricula:/d\n”, Felipe.v_nmat);`  
19`printf(“Media: %2f\n”, Felipe.v_media);`  
20`system(“pause”);`  
21`return(0);`  
22`}`  

Neste Exemplo 5, é declarada a struct aluno, conforme a linha 5 do código-fonte.

A struct aluno é composta pelos campos matrícula, nota e médica, onde o nome do campo matrícula é v\_nmat do tipo int, o nome do campo nota é v\_nota do tipo float e o nome do campo média é v\_media do tipo float. O campo nota é também um vetor de 3 posições, conforme sua declaração na linha 7.

Na linha 12, é declarada a variável Felipe do tipo struct aluno.

A struct aluno Felipe recebe os valores para os seus campos nas linhas 13 a 17. Na linha 13, o campo v\_nmat recebe o valor de 120. Nas linhas 14, 15 e 16, o campo v\_nota, que é um array, recebe os valores para as três posições do vetor.

Na linha 17, para o último campo da struct aluno é calculada a média do aluno e armazenada.

O exemplo finaliza com a impressão da matrícula (linha 18) e da média (linha 19) das notas do aluno Felipe.

Após a execução do programa, temos o retorno com o valor das variáveis ilustradas na Figura 13.

![](img/img_14.jpg "Fonte:Shutterstock")

Figura 13: Saída da execução do Exemplo 5. Fonte: O Autor.

Vamos analisar mais um exemplo.

No caso do Exemplo 6, criamos a struct ficha\_de\_aluno. Depois de criar a struct, precisamos criar a variável que vai utilizá-la. Para tanto, criamos a variável aluno, que será do tipo ficha\_de\_aluno.

Exemplo 6

												
`1 /* Ficha de Aluno */ 2 #include < stdio.h >  3 #include < conio.h > 4 int main(void) 5 { 6 /*Criando a struct */ 7 struct ficha_de_aluno 8 { 9 char nome[50]; 10 char disciplina[30]; 11 float nota_prova1; 12 float nota_prova2; 13 }; 14       15 /*Criando a variável aluno que será do 16 tipo struct ficha_de_aluno */ 17 struct ficha_de_aluno aluno; 18 19 printf("\n---------- Cadastro de aluno -----------\n\n\n");       20 printf("Nome do aluno ......: "); 21 fflush(stdin); 22 fgets(aluno.nome, 40, stdin);       23 printf("Disciplina ......: "); 24 fflush(stdin); 25 fgets(aluno.disciplina, 40, stdin);       26 printf("Informe a 1a. nota ..: ");       27 scanf("%f", &aluno.nota_prova1);       28 printf("Informe a 2a. nota ..: "); 29 scanf("%f", &aluno.nota_prova2);       30 printf("\n\n --------- Lendo os dados da struct ---------\n\n"); 31 printf("Nome ...........: %s", aluno.nome); 32 printf("Disciplina .....: %s", aluno.disciplina); 33 printf("Nota da Prova 1 ...: %.2f\n" , aluno.nota_prova1); 34 printf("Nota da Prova 2 ...: %.2f\n" , aluno.nota_prova2);       35 getch(); 36 return(0); 37 }`
											

No Exemplo 6, é declarada a struct ficha\_de\_aluno composta pelos seguintes campos: Nome, disciplina, nota\_prova1 e nota\_prova2. O campo nome é uma variável do tipo char e um vetor com 50 itens, o campo disciplina é uma variável do tipo char e um vetor com 30 itens e os campos nota\_prova1 e nota\_prova2 são variáveis do tipo float.

Ao continuar com o reconhecimento do código-fonte do Exemplo 6, é observado o uso da instrução fgets() (linhas 22 e 25) com o objetivo de ler strings, no caso, o nome do aluno e a disciplina.

fgets(variavel, tamanho da string, entrada)

Nesse caso, a entrada é stdin (entrada padrão), pois estamos lendo do teclado, mas, em outro caso, a entrada também poderia ser um arquivo.

Continuando, a struct ficha\_de\_aluno aluno recebe os valores para os campos nota\_prova1 e nota\_prova2 nas linhas 27 e 29.

Após a execução do programa, temos o retorno com o valor das variáveis ilustradas na Figura 14.

![](img/img_15.jpg "Fonte: O Autor")

Figura 14: Saída da execução do Exemplo 6. Fonte: O Autor.

Struct aninhada
===============

### Definição

Uma estrutura de dados aninhada ou struct aninhada é basicamente uma estrutura dentro de outra, ou seja, uma estrutura contida em outra ou uma estrutura que pode ser acessada por outra.

Desta maneira, podemos entender que a struct aninhada é um aninhamento de estruturas que nos permite criar estruturas que contenham outras estruturas internas.

O padrão ANSI C especifica que as estruturas de dados (struct) podem ser aninhadas até 15 níveis, mas a maioria dos compiladores permite mais.

### Declaração

Apenas para relembrar, sabemos que a declaração de estrutura declara um tipo struct. E cada tipo struct recebe um nome (ou tag) que se refere àquele tipo pelo nome precedido pela palavra struct. Cada unidade de dados na estrutura é chamada membro e possui um nome de membro. Os membros de uma estrutura podem ser de qualquer tipo. Sendo assim, os membros de estruturas podem ser também outras estruturas.

As estruturas aninhadas podem ser declaradas de duas formas.

A primeira forma é colocar uma estrutura dentro de outra, literalmente. Portanto, a sintaxe para trabalhar com estruturas aninhadas nessa forma é:

	
`typedef struct { 	tipo membro_1; 	tipo membro_2; 	... 	tipo membro_n; 	struct{ 		tipo membro_interno_1; 		tipo membro_interno _2; 		... 		tipo membro_interno _n; 	} } Nome_estrutura; Nome_estrutura NE;`

											

E para acessar os membros, o acesso é direto e a sintaxe é:

												
`//Para atribuir valores: NE.membro_interno_1 = 0; NE.membro_1 = 0;   //Para leitura do teclado: &NE.membro_interno_1 &NE.membro_1  //Para impressão: NE.membro_interno 1 NE.membro_1`
											

A outra forma é você declarar a estrutura\_1 antes e, na estrutura\_2, declarar uma variável da estrutura 1. Desta forma, a sintaxe é a seguinte:

												
`typedef struct { 	tipo membro_1; 	tipo membro_2; 	... 	tipo membro_n; } nome_estrutura_1; 	 typedef struct { 	tipo membro_1; 	tipo membro_2; 	nome_estrutura_1 NE1; 	... 	tipo membro_n; } nome_estrutura_2; 	 nome_estrutura_2 NE2;`
											

E para acessar os membros, a sintaxe é:

												
`//para acessar os membros NE2.membro1; NE2.membro2; NE2.NE1.membro1; NE2.NE1.membro2;`
											
											

Para entendermos melhor as duas formas de declaração de estrutura aninhadas, vamos analisar o Exemplo 7 abaixo.

Exemplo 7

												
`1	 #include < stdio.h > 2	 #include < stdlib.h > 3 4	 struct departamento { 5		 int cod; 6		 char descricao[30]; 7 	}; 8  9 	struct cargo { 10		 int cod; 11		 char descricao[30]; 12 	}; 13  14	 struct funcionario { 15		 int cod; 16 		char nome[30]; 17 		float salario; 18		 struct departamento depto; 19 		struct cargo cargo; 20 	}; 21 22 	struct funcionario Funcionario; 23  24 	int main(void) 25	 { 26 27 	}`
												
											

Observe as linhas de 4 a 20. Nesse trecho, são definidas três estruturas que recebem os nomes: departamento, cargo e funcionário. A estrutura funcionário possui 5 membros, os dois últimos membros são do tipo struct departamento e struct cargo, isto é, dentro da estrutura funcionário, temos dois membros do tipo struct.

Em resumo, temos:

*   Nas linhas 4 e 7, foi declarada a estrutura departamento.
*   Nas linhas 9 e 12, foi declarada a estrutura cargo.
*   Nas linhas 14 e 20, foi declarada a estrutura funcionário.
*   Na linha 18, o campo depto é do tipo struct departamento.
*   Na linha 19, o campo cargo, da mesma forma que o campo depto, é do tipo struct cargo.

Ao analisar o código, visualizamos uma struct aninhada nas linhas 18 e 19, com os campos depto e cargo. Temos, então, um aninhamento de estruturas.

Outra forma de declarar uma estrutura é colocar uma estrutura dentro da outra, literalmente, como apresentado no Exemplo 8 a seguir:

Exemplo 8:

												
`1	 #include < stdio.h > 2 	#include < stdlib.h > 3 4	 struct cargo { 5		 int cod; 6		 char descricao[30]; 7	 }; 8  9	 struct funcionario { 10 		int cod; 11		 char nome[30]; 12 		float salario; 13		 struct departamento { 14 			int cod; 15			 char descricao[30]; 16 		}; 17 18		 struct cargo cargo; 19 	}; 20 21	 struct funcionario Funcionario; 22  23 	int main(void) 24 	{ 25 26 	}`												
											

Além das duas formas de declaração de estrutura aninhada mostradas anteriormente, pode-se utilizar também o tipo typedef ao invés de struct.

Sendo assim, vamos analisar o Exemplo 8 adaptado para o uso de typedef.

Exemplo 8 ‒ adaptado:

												
`1 	#include < stdio.h > 2 	#include < stdlib.h > 3 4	 typedef struct departamento { 5 		int cod; 6 		char descricao[30]; 7	 } Departamento; 8  9 	typedef struct cargo { 10 		int cod; 11 		char descricao[30]; 12	 } Cargo; 13 14 	typedef struct funcionario { 15 		int cod; 16 		char nome[30]; 17 		float salario; 18		 Departamento depto; 19		 Cargo cargo; 20	 } Funcionario; 21 printf( "\n TEXTO %_" , nome_vetor_struct[indice].nome_membro_struct);  22	 int main(void) 23 	{ 24 25	 }`												
											

Ao analisar o código, podemos observar que o typedef foi declarado em conjunto com o struct, tanto para a estrutura departamento quanto para cargo e para a estrutura funcionário. Isto é útil apenas para resumir a codificação, mas não influi no desempenho da aplicação.

### **Comentário**

O comando typedef permite criar um novo nome para outro tipo de dados. Assim, o novo tipo de dados pode ser declarado como um tipo de dados primitivo existente no Linux.

Ao analisar a declaração dos campos depto e cargo, observe que estes campos agora não são mais do tipo estrutura, mas dos tipos definidos **Departamento** e **Cargo**, respectivamente.

Desta forma, pode-se declarar campos de outros tipos definidos dentro de uma estrutura que também pode ser um tipo definido. Além disso, não há uma limitação para o número de níveis na declaração aninhada, contudo, não seria prático incluir muitos níveis, pois isto irá complicar o entendimento para manutenção do código-fonte.

												
`1	 #define LEN 50 2 3	 struct endereco { 4		 char rua[LEN]; 5 		char cidade_estado_cep[LEN]; 6	 }; 7 8	 struct student { 9		 char id[10]; 10		 int idade; 11	 		struct endereco casa; 12		 struct endereco escola; 13	 }; 14 15	 struct student pessoa;`												
											

![icone mão na massa](./img/mao_na_massa_icon.svg)

Mão na Massa
============

### Exemplos práticos

No Exemplo 9, vamos criar uma struct para armazenar os dados do aluno (código, nome e data de nascimento).

    
    1	 #include < stdio.h >
    2	 #include < stdlib.h >
    3	 #include < string.h >
    4	 #include < locale.h >
    5
    6	 typedef struct {
    7	    int codigo;
    8	    char nome[200];
    9		 struct {
    10		       int dia;
    11		       int mes;
    12		       int ano;
    13		 };
    14	 } Aluno;
    15	Aluno aluno;
    16
    17	 	int main(void) {
    18	    setlocale(LC_ALL,"portuguese");
    19	    aluno.codigo = 0;
    20	    strcpy(aluno.nome, "NULL");
    21	    aluno.dia = 0;
    22	    aluno.mes = 0;
    23	    aluno.ano = 0;
    24	    printf(" \n O código do aluno é: %d ", aluno.codigo);
    25	    printf(" \n O nome do aluno é: %s ", aluno.nome);
    26	    printf(" \n A data de nascimento do aluno é: %d / %d / %d ", aluno.dia, aluno.mes, aluno.ano);
    27	    printf(" \n \n");
    28	    printf(" Digite o código do aluno: ");
    29	    scanf("%d%*c", &aluno.codigo);
    30	    printf(" Digite o nome do aluno: ");
    31	    scanf("%s%*c", &aluno.nome);
    32	    printf(" Digite o dia do nascimento do aluno: ");
    33	    scanf("%d%*c", &aluno.dia);
    34	    printf(" Digite o mês do nascimento do aluno: ");
    35	    scanf("%d%*c", &aluno.mes);
    36	    printf(" Digite o ano do nascimento do aluno: ");
    37	    scanf("%d%*c", &aluno.ano);
    38	    printf(" \n O código do aluno é: %d ", aluno.codigo);
    39	    printf(" \n O nome do aluno é: %s ", aluno.nome);
    40	    printf(" \n A data de nascimento do aluno é: %d / %d / %d ", aluno.dia, aluno.mes, aluno.ano);
    41	    printf(" \n \n");
    42	    system("pause");
    43	    return(0);
    44	}
    

Observe as linhas de 06 a 14. Nesse trecho do código-fonte, é definida uma estrutura que recebe o nome de Aluno e, dentro dela, outra estrutura com os membros dia, mês e ano.

A estrutura que possui a data de nascimento do aluno está nas linhas 10, 11 e 12, note que ela não tem nome, e não é necessário que tenha, pois ela está contida dentro da estrutura Aluno. Podemos dizer que temos uma estrutura externa e uma estrutura interna, as quais são respectivamente Aluno e data.

Os membros da estrutura interna são acessados da mesma forma que a estrutura externa, isto é, diretamente.

Na linha 26, podemos observar a forma de acesso diretamente pelo nome da variável da Estrutura.

Agora, no Exemplo 10, vamos criar uma struct para armazenar os dados do aluno (código, nome e data de nascimento), porém, a declaração será diferente do Exemplo 9, pois alguns membros da estrutura são do tipo struct.

												
`#include < stdio.h >  	#include < stdlib.h > 	#include < string.h > 	#include < locale.h > 		 	typedef struct { 		int dia; 		int mes; 		int ano; 	} Data; 		 	typedef struct {  		int codigo; 		char nome[200]; 		Data datNasc; 	} Aluno; 	Aluno aluno; 		 	int main() {  		setlocale(LC_ALL,"portuguese"); 		aluno.codigo = 0; 		strcpy(aluno.nome, "NULL"); 		aluno.datNasc.dia = 0; 		aluno.datNasc.mes = 0; 		aluno.datNasc.ano = 0; 		printf(" \n O código do aluno é: %d ", aluno.codigo); 		printf(" \n O nome do aluno é: %s ", aluno.nome); 		printf(" \n A data de nascimento do aluno é: %d / %d / %d ", aluno.datNasc.dia, aluno.datNasc.mes, aluno.datNasc.ano); 		printf(" \n \n"); 		printf(" Digite o código do aluno: "); 		scanf("%d%*c", &aluno.codigo); 		printf(" Digite o nome do aluno: "); 		scanf("%s%*c", &aluno.nome); 		printf(" Digite o dia do nascimento do aluno: "); 		scanf("%d%*c", &aluno.datNasc.dia); 		printf(" Digite o mês do nascimento do aluno: "); 		scanf("%d%*c", &aluno.datNasc.mes); 		printf(" Digite o ano do nascimento do aluno: "); 		scanf("%d%*c", &aluno.datNasc.ano); 		printf(" \n O código do aluno é: %d ", aluno.codigo); 		printf(" \n O nome do aluno é: %s ", aluno.nome); 		printf(" \n A data de nascimento do aluno é: %d / %d / %d ", aluno.datNasc.dia, aluno.datNasc.mes, aluno.datNasc.ano); 		printf(" \n \n"); 		system("pause"); 		return(0); 	}`												
											

No Exemplo 10, as estruturas são declaradas separadamente. As estruturas que serão utilizadas dentro de outras devem ser declaradas antes.

### **Atenção**

Se você declarar uma estrutura e tentar utilizá-la dentro de outra estrutura, e a estrutura utilizada não tiver sido declarada antes, ao compilar o programa, um erro será apresentado.

Assim, em nosso exemplo, declaramos antes a estrutura data, que será usada dentro da estrutura aluno. Isto é notado nas linhas 6 a 16.

A forma de acesso aos membros da estrutura Aluno agora é um pouco diferente. Dentro da estrutura Aluno, é criada uma variável do tipo da estrutura Data, que é datNasc. Este nome, datNasc, é o nome que deverá ser utilizado para acessar os seus membros. Mas não somente ele, é necessário usar em conjunto com o nome da estrutura aluno, como mostram as linhas 23, 24 e 25.

												
`1 typedef struct { 2         char nome[200]; 3         char disciplina[100]; 4         float nota; 5 } Aluno; 6 7 Aluno aluno_nota[10];`
											

												
`&nome_vetor_struct[indice].nome_membro_struct; 	 For (i=0; i< 10; i++) {     printf(" Digite nome do aluno: ");     scanf("%s%*c", & aluno_nota [i].nome);     printf(" Digite a disciplina do aluno: ");     scanf("%s%*c", & aluno_nota [i].disciplina);     printf(" Digite o nota do aluno: ");     scanf("%f%*c", & aluno_nota [i].nota); }`
											
											

												
`for(i=0; i< 10; i++) { 	printf(" \n O nome do aluno é: %d ", aluno_nota [i].nome); 	printf(" \n A disciplina do aluno é: %d ", aluno_nota [i].disciplina); 	printf(" \n A nota do aluno é: %.2f ", aluno_nota [i].nota); }`													
											

if(strcmp(nome, aluno\_nota \[i\].nome)== 0)

	
`1 #include < stdio.h > 2 #include < stdlib.h > 3 #include < string.h > 4 #include < locale.h > 5  6 typedef struct { 7     int dia; 8     int mes; 9     int ano; 10 } Data; 11  12 typedef struct { 13     int codigo; 14     char nome[200]; 15     Data datNasc; 16 } Aluno; 17   18 Aluno aluno[5]; 19 int i=0; 20  21 int main() { 22     setlocale(LC_ALL,"portuguese"); 23     for(i=0; i< 5; i++) { 24         aluno[i].codigo = 0; 25         strcpy(aluno[i].nome, "NULL"); 26         aluno[i].datNasc.dia = 0; 27        aluno[i].datNasc.mes = 0; 28         aluno[i].datNasc.ano = 0; 29     } 30   31     for(i=0; i< 5; i++) { 32         printf(" \n ======================================================================"); 33         printf(" \n O código do aluno é: %d ", aluno[i].codigo); 34         printf(" \n O nome do aluno é: %s ", aluno[i].nome); 35         printf(" \n A data de nascimento do aluno é: %d / %d / %d ",  36              aluno[i].datNasc.dia, aluno[i].datNasc.mes,  37              aluno[i].datNasc.ano); 38         printf(" \n "); 39     } 40  41     for(i=0; i< 5; i++) { 42         printf(" \n ======================================================================"); 43         printf(" \n ======================================================================"); 44         printf(" \n Digite o código do aluno: "); 45         scanf("%d%*c", &aluno[i].codigo); 46         printf(" \n Digite o nome do aluno: "); 47         scanf("%s%*c", &aluno[i].nome); 48         printf(" \n Digite o dia do nascimento do aluno: "); 49         scanf("%d%*c", &aluno[i].datNasc.dia); 50         printf(" \n Digite o mês do nascimento do aluno: "); 51        scanf("%d%*c", &aluno[i].datNasc.mes); 52        printf(" \n Digite o ano do nascimento do aluno: "); 53         scanf("%d%*c", &aluno[i].datNasc.ano); 54    } 55  56    for(i=0; i< 5; i++) { 57        printf(" \n ======================================================================"); 58        printf(" \n O código do aluno é: %d ", aluno[i].codigo); 59        printf(" \n O nome do aluno é: %s ", aluno[i].nome); 60         printf(" \n A data de nascimento do aluno é: %d / %d / %d ", 61             aluno[i].datNasc.dia, aluno[i].datNasc.mes, 62            aluno[i].datNasc.ano); 63        printf(" \n "); 64    } 65    system("pause"); 66    return(0); 67}`	
		

               `typedf struct time {     char nome[50]; } Time;   struct Jogador {     int nr_camisa;     char nome[30];     Time t; } jogador;`