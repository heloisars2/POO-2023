# Atv09

Você foi contratado para desenvolver um programa em Java que realiza operações com números inteiros. Para isso, você precisa implementar métodos sem retorno que executam tarefas específicas. 


- Implemente o método imprimirNumeros, que recebe um array com 10 inteiros como parâmetro e exibe os números na tela, separados por um espaço. O método não deve retornar nenhum valor.


- Implemente o método somaNumeros, que recebe um array com 10 inteiros como parâmetro, calcula a soma de todos os números do array e exibe o resultado na tela. O método não deve retornar nenhum valor 


- No método main, um array de números inteiros é criado e inicializado. Você deve chamar o método imprimirNumeros passando o array como argumento. Em seguida, chame o método somaNumeros para calcular a soma dos números e exibir o resultado. Por fim, chame novamente o método imprimirNumeros para exibir o array atualizado após a soma.

Observações:
Os métodos imprimirNumeros e somaNumeros devem ser implementados dentro da classe ExercicioSemRetorno.
Utilize estruturas de repetição e operações matemáticas para calcular a soma dos números.

```
/*Classe: Atv01.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */ 

public class ATV09{// Declaração da classe Atv09
   
   public static void main(String[] args) {// Declaracao do método main 
       
       int[] v01 = {123, 32, 1, 5, 7, 4, 86, 1, 3, 10};//declaração e inicializacao do vetor 'v01' 

       //chamando o metodo imprimirNumeros para printar o array 
       imprimirNumeros(vetor);

       int[] v02 = {32, 23, 12, 54, 2, 3, 1, 2, 3, 0};//declaração e inicializacao do vetor 'v02' 

       soma(v01, v02);
       
   } // fim do metodo main
   
   // Declaração do método imprimir que imprime os números
   public static void imprimir(int[] array) {
       System.out.println("Saida do Vetor: ");
       //percorre o vetor e faz um print de cada posição
       for (int i = 0; i < array.length; i++) {
           System.out.print(array[i] + "\t");
       }
       
       System.out.println();//quebra de linha
   } // fim do imprimir

   //método soma dois array como parametro 
   public static void soma (int[] array, int[] array2) {
       //declara vetor "array" com o tamanho do vetor "v01"
       int[] arrayParaSoma = new int[array.length];

       //soma os array e atribuindo o valor para outro arrray
       for (int i = 0; i < array.length; i++) {
           arrayParaSoma[i] = array[i] + array2[i];
       }

       //prints de orientação
       System.out.println();
       System.out.println("Saida do vetor somado");
       //chama o metodo imprimir para printar a soma dos array
       imprimir(arrayParaSoma);
   } // fim do metodo soma

}// fim da classe Atv09

```
