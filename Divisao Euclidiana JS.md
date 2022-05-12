# Desafio
Você recebeu desafio de desenvolver um programa que calcule o quociente e o resto da divisão de dois números inteiros. Não se esqueça que o quociente e o resto da divisão de um inteiro a por um inteiro não-nulo b são respectivamente os únicos inteiros q e r tais que:

0 ≤ r < |b|

Se r < 0: r = r - |b|

a = b × q + r

q = ( a - r ) / b

Caso você não saiba, o teorema que garante a existência e a unicidade dos inteiros q e r é conhecido como ‘Teorema da Divisão Euclidiana’ ou ‘Algoritmo da Divisão’.

**  |b| (Módulo / Valor absoluto): É o valor representado de forma positiva;

# Entrada
A entrada é composta por dois números inteiros a e b (-1.000 ≤ a, b < 1.000).

# Saída
Imprima o quociente q seguido pelo resto r da divisão de a por b, considerando as regras apresentadas a cima.

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados e a função print para imprimir a saída (output) de dados.
// Abaixo segue um exemplo de código que você pode ou não utilizar

let line = gets().split(" ");
const a = parseInt(line[0]);
const b = parseInt(line[1]);

q = parseInt(a / b);
r = a - b * q;

if (r < 0) {
  r += Math.abs(b);
  
  q = (a-r)/b;    //Aplicação Teorema da divisao Euclidiana
}

print(q + " " + r);