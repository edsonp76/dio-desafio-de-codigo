# Desafio
Crie um programa onde você receberá valores inteiros não negativos como entrada.

Ordene estes valores de acordo com o seguinte critério:

Primeiro os Pares
Depois os Ímpares
Você deve exibir os pares em ordem crescente e na sequência os ímpares em ordem decrescente.

# Entrada
A primeira linha de entrada contém um único inteiro positivo N (1 < N < 10000) Este é o número de linhas de entrada que vem logo a seguir. As próximas N linhas terão, cada uma delas, um valor inteiro não negativo.

# Saída
Exiba todos os valores lidos na entrada segundo a ordem apresentada acima. Cada número deve ser impresso em uma linha, conforme exemplo de saída abaixo.

 
# Exemplo de Entrada
10
4
32
34
543
3456
654
567
87
6789
98

#  Exemplo Saida
4
32
34
98
654
3456
6789
567
543
87

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados
// Abaixo segue um exemplo de código que você pode ou não utilizar

var num = parseInt(gets());
var index = 0;

var numeros = Array(num);

while (index < num ) {
  
  numero = parseInt(gets());
  
  if (numero >= 0 ) {
    numeros[index] = numero;
    index++;
  }

}

pares = numeros.filter(value => value % 2 == 0);
impares = numeros.filter(value => value % 2 != 0);

pares.sort((a, b) => a-b);
impares.sort((a, b) => b-a);

pares.forEach(i => console.log(i));
impares.forEach(i => console.log(i));


