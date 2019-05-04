# Análise de Algoritmos

### Problema 1
Quais são as duas características mais comuns para analisar algoritmos?
**R**: Tempo de execução e consumo de memória.

### Problema 2
Por que a medida de tempo em segundos não representa qualiﬁcadamente o tempo de execução de um algoritmo?

**R**: A quantidade de segundos a qual um algoritmo é executado depende do equipamento computacional assim como o contexto aplicado. Por exemplo, com uma máquina mais potente pode se obter com um mesmo algoritmo um resultado em tempo de execução inferior. Assim como, por exemplo, no contexto  de um algoritmo de cálculo de trajetória balística horas de execução é um valor aceitável (porém, não é para aplicações mais genéricas).

### Problema 3
A medida de tempo de um algoritmo é realizada através de qual informação? O que pode afetá-la?

**R**: A medida de tempo é realizada de acordo com a quantidade de passos necessários para o algoritmo ser executado. O tamanho da entrada e o ambiente externo (hardware) são as principais causas que podem afeta-lo.

### Problema 4
Na análise de algoritmos, qual é o valor da base da função logarítmica e exponencial? Por que é escolhido este valor?

**R**: Na logarítmica e na exponencial se utiliza base 2, que representa as possíveis variações de um binário.

### Problema 5
O que é complexidade de tempo?

**R**: Complexidade de tempo expressa a quantidade de tempo gasta para rodar um algoritmo em função da entrada da função.

### Problema 6
Dado dois algoritmos *A* e *B* com as complexidades de tempo respectivamente *f1* e *f2*, qual é o melhor algoritmo? O que indica qual é o melhor algoritmo?

**R**: Aquele que possuir a menor complexidade de tempo, ou seja, a menor quantidade de etapas executadas.

### Problema 7
Em uma função de complexidade, o que representa o termo *n*?

**R**: O n dentro de uma função de complexidade representa o tamanho da entrada.

### Problema 8
Quais são as operações primitivas de um algoritmo?

**R**: As operações:
atribuição de valores a variáveis, 
chamadas de métodos, 
operações aritméticas,
comparação entre valores, 
Acesso a um vetor, 
Ponteiro para um objeto 
retorno de um método.

### Problema 9
Qual é o valor de uma operação primitiva de um algoritmo?

**R**: Sempre 1.

### Problema 10
Desenvolva o pseudocódigo do algoritmo *SOMA*, que realiza a soma de dois números inteiros recebidos por parâmetro e tem como saída a resultado da operação. Identiﬁque a sua função de complexidade de tempo.

~~~~
SOMA (NUMERO1, NUMERO2)
  SOMA ← NUMERO1 + NUMERO2
  RETORNA SOMA  
~~~~

**Complexidade de tempo:** f(n) = c1 * n + c2 *n = 1

### Problema 11
Desenvolva o pseudocódigo do algoritmo *SOMA VETOR*, que realiza a soma de todos os elementos de um vetor. O algoritmo recebe o vetor *V* e tem como saída o resultado. Identiﬁque a sua função de complexidade de tempo.

~~~~
SOMA_VETOR (V)
	TOTAL ← 0
  PARA I ← 1 ATÉ N
      TOTAL ← TOTAL + V[I]
    RETORNA TOTAL
~~~~


**Complexidade de tempo:** f(n) = c1 * n + c2 * n + c3 * n + c4 * n = 1 + n + n + 1 = 2n + 2

### Problema 12
Desenvolva o pseudocódigo do algoritmo *CONTAGEM IMPARES*, que realiza a contagem de números impares de um vetor. O algoritmo recebe o vetor *V* e tem como saída o resultado. Identiﬁque a sua função de complexidade de tempo.

~~~~
CONTAGEM_IMPARES (V)
	IMPARES ← 0
	PARA I ← 1 ATÉ N
		SE V[I] % 2 != 0 ENTÃO
			IMPARES ← IMPARES + 1
	RETORNA IMPARES
~~~~

**Complexidade de tempo:** f(n) = c1 * n + c2 * n + c3 * n + c4 * n + c5 * n = 1 + n + n + n + 1 = 3n + 2

### Problema 13
Desenvolva o pseudocódigo do algoritmo *SOMA MATRIZ*, que realiza a soma de todos os elementos de uma matriz. O algoritmo recebe a matriz *M* e tem como saída o resultado. Identiﬁque a sua função de complexidade de tempo.

~~~~
SOMA_MATRIZ (M)
	SOMA ← 0
	PARA I ← 1 ATÉ N
		PARA J ← 1 ATÉ N
			SOMA ← SOMA + M[I][J]
	RETORNA SOMA
~~~~

**Complexidade de tempo:** f(n) = c1 * n + c2 * n + c3 * n + c4 * n + c5 * n = 1 + n + n*n + n*n + 1 = 2n² + n + 1

### Problema 14
Desenvolva o pseudocódigo do algoritmo *BUSCA MATRIZ*, que identiﬁca posição *x* e *y* de um elemento em uma matriz. O algoritmo recebe a matriz *M* e o valor *V* e tem como saída a posição *x* e *y* . Identiﬁque a sua função de complexidade de tempo.

~~~~
BUSCA_MATRIZ(M, V)
	POS ← [2]
	PARA I ← 1 ATÉ N
		PARA J ← 1 ATÉ N
			SE M[I][J] = V ENTÃO
				POS[0] ← I
				POS[1] ← M
	RETORNA POS
~~~~

**Complexidade de tempo:** f(n) = c1 * n + c2 * n + c3 * n + c4 * n + c5 * n + c6 * n + c7 * n = 1 + n + n² + n² + n² + n² + 1 = 4n² + n + 2

### Problema 15
O que é análise assintótica? Qual é o seu objetivo?

**R**: Análise assintótica é uma técnica utilizada para analisar um algoritmo que recebe grandes entradas de dados, de forma a prover uma estimativa de complexidade.

### Problema 16
Qual é o processo da análise assintótica? Crie um exemplo.

**R**:

O processo da análise assintótica é o seguinte:
-Identificação da complexidade do algoritmo;

~~~~
Ex: f(n) = 6n³ + 2n² + n + 5
~~~~

-Identificação do componente de maior ordem;

~~~~
Ex: 6n³
~~~~
-Ignoração do coeficiente do elemento de maior ordem;

~~~~
Ex: n³
~~~~

### Problema 17
O que é a notação assintótica?

**R**: A notação assintótica é um tipo de notação utilizada para analisar algoritmos que recebem uma entrada de dados muito grande, assim é utilizada esse tipo de notação para examinar algoritmos bem complexo. Nesta notação é considerado apenas a variável de maior grau (sem considerar à constante também).

### Problema 18
O que é a notação O-Grande ou Big-Oh?

**R**: O Big Oh é uma notação assintótica que serve para descrever relações onde uma função é maior ou igual a outra.

### Problema 19
Qual é a deﬁnição formal da notação O-Grande?

**R**: O Big Oh segue formalmente o seguinte princípio: f(n) = O(g(n)) quando f(n) <= Kg(n) (onde “K” é uma constante qualquer).


### Problema 21
O que é a notação o-pequeno ou Little-Oh?

**R**: A Little Oh é uma notação assintótica que serve para descrever relações onde uma função é menor que a outra.

### Problema 22
Qual é a deﬁnição formal da notação o-pequeno?
**R**: A Little Oh segue formalmente o seguinte princípio: f(n) = o(g(n)) onde f(n) > Kg(n) (onde “K” é uma constante qualquer).

### Problema 24
Passe a notação O-grande e o-pequeno as funções abaixo:

**A**) *F(n) = n + 1*
**B**) *Fn) = 8*
**C**) *F(n) = 2n<sup>2</sup> −1*
**D**) *F(n) = nlogn*
**E**) *F(n) = 3n! + 2n*
**F**) *F(n) = 3n<sup>3</sup> + 2n<sup>2</sup> + 4n + 6*
**G**) *F(n) = 5<sup>n</sup> + 11*
**H**) *F(n) = 3logn*

| N° |       Big Oh       |     Little Oh      |
|:--:|:------------------:|:------------------:|
|  1 |   O(n)             |   o(n)             |
|  2 |   O(1)             |   o(1)             |
|  3 |   O(n²)            |   o(n²)            |
|  4 |  O(nlog n)         |   o(nlog n)        |
|  5 |   O(n!)            |   o(n!)            |
|  6 |   O(n³)            |   o(n³)            |
|  7 |   O(5<sup>n</sup>) |   o(5<sup>n</sup>) |
|  8 |  O(log n)          |     o(log n)       |

### Problema 25
Identiﬁque o O-Grande dos algoritmos desenvolvidos nos Problemas 10 até 14.
10) O(1)
11) O(n)
12) O(n)
13) O(n²)
14) O(n²)
