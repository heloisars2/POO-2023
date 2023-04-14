# Atv02

Crie uma classe em Java que realize cada uma das seguintes tarefas:
a) Exibir a mensagem “Informe um inteiro: “, deixando o cursor na mesma linha;
b) Atribuir o produto de variáveis b e c para a variável a;
c) Utilizar um comentário para afirmar que um programa executa um cálculo de exemplo de folha de pagamento.

```
/*Classe de impresão de texto: Atv01.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */

import java.util.Scanner; //importa classe Scanner  

public class Atv02 {// Declara a classe Atv02
	public static void main(String[] args) {
        Scanner h = new Scanner(System.in); //prepara a entrada de dados
        
        System.out.println("Digite um valor:"); //informa ao usuario oque ele precisa informar
        int b = h.nextInt(); //declara e inicializa a variavel
        int c = 2;
        
        h.close(); // fecha o objeto h
        
        
        int a = b * c; //declara a variavel a e faz a multiplicação de b e c
        
        System.out.println("O produto é: " + a);//exibe o resultado na tela
	}
}//fim da classe Atv02
```
