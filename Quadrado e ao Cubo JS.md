# Desafio
Você terá o desafio de escrever um programa que leia um valor inteiro N (1 < N < 1000). Este N é a quantidade de linhas de saída que serão apresentadas na execução do programa.

# Entrada
O arquivo de entrada contém um número inteiro positivo N.

# Saída
Imprima a saída conforme o exemplo fornecido.

 
# Exemplo de Entrada	
5

# Exemplo de Saída
1 1 1
2 4 8
3 9 27
4 16 64
5 25 125

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados e a função print para imprimir a saída (output) de dados.
// Abaixo segue um exemplo de código que você pode ou não utilizar

//let linhas = parseInt(gets());

//TODO: Complete os espaços em branco com uma solução possível para o problema.

let limit = parseInt(gets());

//for (let i = 1; i <= limit; i++) {
 // let X =parseInt(gets(i**2));
  //let Y =parseInt(gets(i**3));

  //console.log(i,X,Y);
//}

for (let i = 1; i <= limit; i++) {
    
    x = i * i
    y = i * i * i
    
    console.log(i, x, y)
}

