# Atv06

objetivo do código:
Dados os valores de um depósito fixo mensal e um montante desejado, crie uma classe para determinar quantos meses serão necessários para acumular o montante desejado, considerando juros mensais de 0,5%.

```
/*Classe de impresão de texto: Atv06.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */ 
 
import java.util.Scanner;
public class Atv06 // Declaração da classe Atv06
{
    public static void main(String[] args) {// Declaracao do método main 
		Scanner h = new Scanner(System.in); //prepara a entrada de dados 
		
        System.out.println("Depositos mensais: "); //mensagem de orientação
		double deposito = h.nextDouble(); //delcrando e atribuindo valores as variaveis
		
		System.out.println("montante desejado: "); //mensagem de orientação
		double montante = h.nextDouble(); //delcrando e atribuindo valores as variaveis
		
		double montante_atual = 0; //declaração e inicialização da variavel
		
		int meses_necessarios = 0; //declaração e inicialização da variavel 
		
		while (montante_atual < montante_desejado){
		    meses_necessarios++; //meses_necessarios recebe mais um para considerar que se passou um mes
		    
		    montante_atual += deposito + (montante_atual * 0.05); 
		    //atualizando o montante_atual com o valor depositado mensalmente mais 5% de juros mensais 
		    
		    System.out.println("Mês:" + meses_necessarios + ", montante_atual = " + montante_atual);
		}
		
		System.out.println(); //organizando a visualização da saida
		
		System.out.println("São necessarios " + meses_necessarios + " meses para alcançar o montante de: " + montante_desejado);
		System.out.println("Com juros mensais de: 5%");
		
	}
} // fim da classe Atv06

```
