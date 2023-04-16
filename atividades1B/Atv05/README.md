# Atv05

Objetivo do código:
Adicione a Atv04 (sem alterar as linhas existentes) o cálculo para a média mensal de gastos, criando uma variável mediaMensal junto com uma mensagem. Para isso, concatene a String com o valor, usando "Valor da média mensal = " + mediaMensal.


```
/*Classe de impresão de texto: Atv05.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */ 
 public class Atv05 {// Declara a classe 
     public static void main(String[] args){
         
         double gastosJaneiro = 30000,00//declara e inicializa a variavel gastosJaneiro
         double gastosFevereiro = 33030,77//declara e inicializa a variavel gastosFevereiro
         double gastosMarco =  23.899,01//declara e inicializa a variavel gastosMarco
         double gastoTotal = gastosJaneiro + gastosFevereiro + gastosMarco; //declara e inicializa a variavel gastoTotal
         double mediaMensal = gastoTotal/3 //declara e incializa a variavel mediaMensal

         // Exibe o valor da soma
         System.out.println("A soma dos gastos mensais é : " + gastoTotal); //mosta na tela o resultado
         System.out.println("A média dos gastos mensais é : " + mediaMensal);//mosta na tela o resultado
     }
 }//fim da classe Atv04
 
```
