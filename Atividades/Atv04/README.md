/*Este algoritmo devolve a soma do balanco  trimestral */


package atv4;

import java.text.DecimalFormat; 

public class BalancoTrimestral { // classe principal

   public static void main(String[] args) {
        
    double gastosJaneiro = 30000.00,  // variaveis usadas para somar
    gastosFevereiro =  33030.77,
    gastosMarco = 23899.01,
    gastosTrimestre;

    DecimalFormat dFormat = new DecimalFormat();// transforma um inteiro em decimal
    

    gastosTrimestre = (gastosJaneiro + gastosFevereiro + gastosMarco); // variavel para somar os gastos

    System.out.println(" Os gastos trimestrais sao : "+"R$"+dFormat.format(gastosTrimestre)); // saida ja com format monetario.
        
    }
    
}


* feito completo depois desmembrada para atender a atividade