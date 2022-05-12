# Desafio
Você terá o desafio de ler um valor inteiro correspondente à idade de uma pessoa em dias e informe-a em anos, meses e dias

Obs.: apenas para facilitar o cálculo, considere todo ano com 365 dias e todo mês com 30 dias. Nos casos de teste nunca haverá uma situação que permite 12 meses e alguns dias, como 360, 363 ou 364. 

# Entrada
O arquivo de entrada contém um valor inteiro.

# Saída
Imprima a saída conforme exemplo fornecido.

# Exemplo de Entrada
400

# Exemplo de Saída
1 ano(s)
1 mes(es)
5 dia(s)

// a função gets é implementada dentro do sistema para ler as entradas(inputs) dos dados
// Abaixo segue um exemplo de código que você pode ou não utilizar

let totalDeDias = parseInt(gets());

let qtAnos = parseInt(totalDeDias / 365)
let qtMeses = parseInt((totalDeDias % 365) / 30);
let qtDias = ((totalDeDias % 365) % 30);

console.log(`${qtAnos} ano(s)\n${qtMeses} mes(es)\n${qtDias} dia(s)`);

