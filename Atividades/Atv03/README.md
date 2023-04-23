/* Esse programa requer que o  usuario insira 3 numeros e devolve a media entre eles ultilizando o metodo
 * JOptionPane.
 */



package atv3;

import javax.swing.JOptionPane;

public class Media {    // classe do codigo
    public static void main(String[] args) {
        String resp = "";                     // string para guardar o numero digitado.
        float nota1,nota2,trabalho,media;     // variaveis  do codigo.
        try{
        resp = JOptionPane.showInputDialog("entre com a nota1"); // eNtrada do usuario no modo box do OPtionPane.
        nota1 = Float.parseFloat(resp);                                  // a nota e transformada em float.

        resp = JOptionPane.showInputDialog("entre com a nota2");
        nota2 = Float.parseFloat(resp);

        resp = JOptionPane.showInputDialog("entre com a nota do trabalho");
        trabalho = Float.parseFloat(resp);

        media = (nota1 + nota2 + trabalho) / 3;                      // variavel que faz a soma depois divide pelas notas.
        JOptionPane.showMessageDialog(null,"media" + Math.round(media)); // aqui sai a resposta 
        }catch(NumberFormatException erro){
            JOptionPane.showMessageDialog(null,"Erro apenas numeros" + erro.toString()); // mensagem de erro caso a entrada nao seja um  numero.

        }
        System.exit(0);// fechamento do codigo
    }
} 