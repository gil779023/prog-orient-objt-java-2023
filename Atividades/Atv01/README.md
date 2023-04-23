package atv1;



    /*Este Algoritmo recebe dois numeros emitidos pelo usuario tanto inteiros
  como decimais e os soma mostrando posterirmente seu resultado */


import java.util.Scanner; // import da bliblioteca scanner

public class Soma {       // classe principal

    public static void main(String[] args) {
        Float n1,n2,sum;        // declaracao de variaveis

        try (Scanner numero1 = new Scanner(System.in)) { // metodo scanner de entrada de usuario
            System.out.println("Primeiro numero :");

            n1 = numero1.nextFloat();                   // variavel recebe uma string e transforma em float.        
            try (Scanner numero2 = new Scanner(System.in)) {
                System.out.println("Segundo numero :");

                n2 = numero2.nextFloat();
            }
            sum = n1 + n2;                          // variavel que recebe os floats e faz a soma.
        }
        System.out.println("resultado e : "+ sum);  // resultado de saida na tela

       
        
        System.exit(0); // fim do codigo

}
    
}