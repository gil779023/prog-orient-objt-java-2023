package atv5;
import java.text.DecimalFormat; 
public class mediaMensal {
 
   public static void main(String[] args) {
        
    double gastosJaneiro = 30000.00,  // variaveis usadas para somar
    gastosFevereiro =  33030.77,
    gastosMarco = 23899.01,
    gastosTrimestre,
    mediaMensal;

    DecimalFormat dFormat = new DecimalFormat("0.00");// transforma um inteiro em decimal
    

    gastosTrimestre = (gastosJaneiro + gastosFevereiro + gastosMarco); // variavel para somar os gastos

    mediaMensal = (gastosJaneiro + gastosFevereiro + gastosMarco) / 3;
    System.out.println(" Os gastos trimestrais sao : "+"R$"+dFormat.format(gastosTrimestre)); // saida ja com format monetario.
    System.out.println("Valor da média mensal = " + "R$"+dFormat.format(mediaMensal));
        
    }
    
}

atividade comentada