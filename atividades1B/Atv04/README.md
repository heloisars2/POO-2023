# Atv04
objetivo do código: 
Atualmente os gastos mensais de uma empresa são detalhados em planilhas eletrônicas. Assim, para fechar o balanço do
primeiro trimestre, é necessário somar o gasto total destas planilhas. Sabendo que, em janeiro, foram gastos R$ 30.000,00 reais, em fevereiro, R$ 33.030,77 reais e em março, R$ 23.899,01 reais, faça uma classe em Java que calcule e exiba o gasto total no trimestre, seguindo os seguintes passos:

a) Crie uma classe chamada BalancoTrimestral com o método main;
b) No método principal, declare uma variável do tipo real chamada gastosJaneiro e inicialize-a com o valor gasto no mês de janeiro;
c) Crie também as variáveis gastosFevereiro e gastosMarco, inicializando-as com os respectivos gastos, utilize uma linha para cada declaração;
d) Crie uma variável chamada gastosTrimestre e inicialize-a com a soma das outras variáveis;
e) Exiba a variável gastosTrimestre.

```
/*Classe de impresão de texto: Atv04.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */ 
 public class Atv04 {// Declara a classe 
     public static void main(String[] args){

         double gastosJaneiro = 30000.00 //declara e inicializa a variavel
         double gastosFevereiro = 33030.77//declara e inicializa a variavel
         double gastosMarco =  23899.01//declara e inicializa a variavel    
         double gastoTrimestre = gastosJaneiro + gastosFevereiro + gastosMarco; //declara a variavel soma e inicializa a soma
         
         // Exibe o valor da soma
         System.out.println("A soma dos gastos mensais é : " + gastoTrimestre);
     }
 }//fim da classe Atv04

```
