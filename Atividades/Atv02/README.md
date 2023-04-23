#feito tudo em um depois dividido em partes para atender os exercicios.


/*esse algoritmo pede que o usuario informe dois numeros e devolve o produto */


package atv2;

import java.util.Scanner;

public class tarefa {

    public static void main(String[] args) {
        int A,B,C;                                    // declaracao de variaveis
        try (Scanner numero = new Scanner(System.in)) {  // metodo onde o usuario  insere dados.
            System.out.print("Informe um Inteiro : ");
            
            C = numero.nextInt();                        // variaveis que transforma uma string em inteiro.
            B = numero.nextInt();                        // variaveis que transforma uma string em inteiro.
        }
        A = (C * B);                                     // variavel que faz a multiplicacao 
        System.out.println(A);                          //  resultado de saida na tela
        System.exit(A);
    }
    
}