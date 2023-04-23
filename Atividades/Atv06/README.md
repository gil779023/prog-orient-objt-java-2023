/*Este algoritmo calcula a quantidade de meses necessarios para atigir um montante com 5% de juros ao mes */

package atv6;
import java.util.Scanner;
public class Deposito { //classe principal
    
    public static void main(String[] args) {
        try (Scanner input = new Scanner(System.in)) {
            System.out.print("Informe o valor do depósito fixo mensal: "); //usuario define o valor do deposito.
            double depositoMensal = input.nextDouble();

            System.out.print("Informe o montante desejado: "); // usuario define o valor do montante.
            double montanteDesejado = input.nextDouble();

            final double juros = 0.005; // 0,5% de juros mensais
            double saldo = 0;
            int meses = 0;

            while (saldo < montanteDesejado) {  //repeticao usada para percorrer dados de incremento.
                saldo += depositoMensal;
                saldo += saldo * juros;
                meses++;
            }

            System.out.println("Serão necessários " + meses + " meses para acumular o montante desejado.");//saida de dados
        }
        System.exit(0);
    }
}
   
 atividade comentada.  