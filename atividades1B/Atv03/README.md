# Atv03

Objetivo do código:
Usando a classe JOptionPane para entrada de dados, crie uma classe que receba a nota de duas provas e de um trabalho. Calcule e mostre a média.

```
/*Classe de impresão de texto: Atv03.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */

import javax.swing.JOptionPane;// importa classe JOptionPane

public class Atv03 {// Declara a classe 
	public static void main(String[] args) {
        String aux;//variavel auxiliar
        float nota1, nota2, nota3;//declara as variaveis
        
        aux = JOptionPane.showInputDialog(null, "Primeira nota");//entrada de dados com a classe JOptionPane
        nota1 = Float.parseFloat(aux);//transforma a string em float e armazena na variavel
        aux = JOptionPane.showInputDialog(null, "Segunda nota");//entrada de dados com a classe JOptionPane
        nota2 = Float.parseFloat(aux);//transforma a string em float e armazena na variavel
        aux = JOptionPane.showInputDialog(null, "Terceira nota");//entrada de dados com a classe JOptionPane
        nota3 = Float.parseFloat(aux); //transforma a string em float e armazena na variavel
        

        
        
        float media = (nota1 + nota2 + nota3)/3 ; //declara a variavel soma e inicializa a soma
        
        // Exibe o valor da soma
        JOptionPane.showMessageDialog(null, "Média = "+ media);
	}
}//fim da classe Atv03
```
