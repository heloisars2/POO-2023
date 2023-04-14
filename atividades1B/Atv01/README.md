# Atv01

* Objetivo da atividade: Criar uma classe em Java que seja capaz de apresentar a soma de todos os argumentos inteiros ou reais recebidos. Argumentos inválidos devem ser desconsiderados sem provocar a exibição de erros ou exceções.



```
/*Classe de impresão de texto: AtvTeste.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */
 
import java.util.Scanner; //importa classe Scanner 
import java.io.IOException;// importa classe IOException 

public class Atv01 {// Declara a classe 
	public static void main(String[] args) throws IOException {
        Scanner h = new Scanner(System.in); //prepara a entrada de dados
        
        System.out.println("Digite dois valores para serem somados:"); //informa ao usuario oque ele precisa informar
        int num_1 = h.nextInt(); //declara e inicializa a variavel
        int num_2 = h.nextInt(); //declara e inicializa a variavel
        
        h.close(); // fecha o objeto h
        
        
        int soma = num_1 + num_2; //declara a variavel soma e inicializa a soma
        
        // Exibe o valor da soma
        System.out.println("A soma dos argumentos é : " + soma);
	}
}//fim da classe Atv01
```
