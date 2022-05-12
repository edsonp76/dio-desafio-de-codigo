#  Desafio
Você deve fazer a leitura de 5 valores inteiros. Em seguida mostre quantos valores informados são pares, quantos valores informados são ímpares, quantos valores informados são positivos e quantos valores informados são negativos. Considere que o número zero é positivo, mas não pode ser considerado como positivo ou negativo.

# Entrada
Você receberá 5 valores inteiros.

# Saída
Exiba a mensagem conforme o exemplo de saída abaixo, sendo uma mensagem por linha e não esquecendo o final de linha após cada uma.

# Exemplo de Entrada
-5
0
-3
-4
12

# Exemplo de Saída
3 par(es)
2 impar(es)
1 positivo(s)
3 negativo(s)

import java.io.IOException;
import java.util.Scanner;

public class minhaClasse {
	
    public static void main(String[] args) throws IOException {
        Scanner leitor = new Scanner(System.in);
//declare suas variaveis corretamente
        int  par = 0;
        int  impar = 0;
        int  positivo = 0;
        int  negativo = 0;
        

//continue a solução

        for (int i = 0; i < 5; i++) {
        	 int n = leitor.nextInt();
        	 
        	 if(n % 2 == 0) par++;
        	 else impar++;
        	 
        	 if(n > 0) positivo++;
        	 else 
        	 if(n == 0) positivo = positivo;
        	 else negativo++;
        }
        

//insira suas variaveis corretamente
        System.out.println( par + " par(es)");
        System.out.println( impar + " impar(es)");
        System.out.println( positivo + " positivo(s)");
        System.out.println( negativo + " negativo(s)");
    }
	
}