# Atv 08

Uma pequena companhia aérea acabou de comprar um computador para seu novo sistema automatizado de reservas. Você foi solicitado a desenvolver o novo sistema. Você escreverá um aplicativo para atribuir assentos em cada voo da companhia aérea (capacidade: 10 assentos).
O sistema deve exibir as seguintes alternativas: 

- Por favor digite 1 para Primeira Classe e digite 2 para Classe Econômica .  Se o usuário digitar 1, o sistema deve atribuir assentos na primeira classe (poltronas 1 a 5). Se o usuário digitar 2, o sistema deve atribuir um assento na classe econômica (poltronas 6 a 10). 

- O sistema deve ainda exibir um cartão de embarque indicando o número da poltrona da pessoa e se ela está na primeira classe ou na classe econômica.

- Utilize um array unidimensional do tipo primitivo boolean para representar o gráfico de assentos do avião. 

- Inicialize todos os elementos do array como false para indicar que todas as poltronas estão desocupadas. 

- À medida que cada assento é atribuído, configure o elemento correspondente do array como true para indicar que o assento não está mais disponível.

- O sistema nunca deve atribuir uma poltrona que já foi reservada. 

- Quando a classe econômica estiver lotada, o sistema deve perguntar à pessoa se ela aceita ficar na primeira classe (e vice-versa). Se sim, faça a atribuição apropriada de assento. Se não, exiba a mensagem "O próximo voo parte em 3 horas".

```
/*Classe: Atv08.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */ 


import java.util.Scanner;//importa a classe Scanner 

public class Atv08//cria a classe Atv08
{
    final static Scanner leitor = new Scanner(System.in); //prepara a entrada de dados
    final static String nomesClientes[] = new String[10]; //alocação do vetor assentos 
    final static boolean assentos[] = new boolean[10]; //alocação do vetor assentos 


    public static void CompraAssento(){
        System.out.println("Digite 1 para Primeira Classe e digite 2 para Classe Econômica");//informa ao usuario oque ele deve inserir

        int entrada = leitor.nextInt();//entrada para a classe de compra

        if (entrada == 1){ //caso entrada seja igual a primeira classe
            int i = 0;
            boolean achouAssento = true; //se tiver acentos é true(verdadeiro)

            do{
                if (i == 5){ //5 assentos na classe
                    System.out.println("A Primeira Classe está cheia");//informa se a classe setá cheia
                    break;//encera o if
                }

                if (assentos[i] == false){//se o acento estiver vazio
                    System.out.println("qual nome deve ser atribuido na compra?");//recebe o nome de quem comprou o acento
                    String nomeCliente = leitor.next();
                    nomesClientes[i] = nomeCliente;
                    assentos[i] = true;
                    achouAssento = false;
                } else{
                    i += 1;//passa pra posição seguinte
                }

            }while(achouAssento);//enquanto achar o assento

        }
        if (entrada == 2){ //caso entrada seja igual a classe economica
            int i = 5;
            boolean achouAssento = true;

            do{
                if (i == 9){ //5 assentos na classe
                    System.out.println("A Classe Economica está cheia");//informa se a classe setá cheia
                    break;
                }

                if (assentos[i] == false){
                    System.out.println("qual nome deve ser atribuido na compra?");//recebe o nome de quem comprou o acento
                    String nomeCliente = leitor.next();
                    nomesClientes[i] = nomeCliente;
                    assentos[i] = true;
                    achouAssento = false;
                } else{
                    i += 1;//passa pra posição seguinte
                }

            }while(achouAssento);

        }

        
    }
 
    public static void main(String[] args) {//classe que mostra os assentos vendidos
        
        for (int i = 0; i<10; i++){//percorre os assentos vendidos e não vendidos

            System.out.println("ASSENTOS");//printa "ASSENTOS"
            System.out.println("primeira classe: ");//informa os assentos da primeira classe
            for(int a = 0; a<10; a++){
                System.out.println(assentos[a]+ "\t"+ nomesClientes[a]);
                if (a == 4){
                System.out.println("classe economica: ");//informa os assentos da classe economica
                }
        }

            CompraAssento();
        }

    }


    
}// encerra a classe Atv08
``
