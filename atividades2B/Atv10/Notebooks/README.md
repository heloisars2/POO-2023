# Atv10

- Crie uma classe chamada "Pessoa" com os seguintes atributos privados: "nome" (do tipo String), "idade" (do tipo int) e "altura" (do tipo double). Em seguida, implemente métodos públicos para acessar e modificar esses atributos, respeitando o princípio de encapsulamento.

- Crie uma classe para testar o funcionamento da classe "Pessoa".

- ```
  /*Classe: Pessoa.java
 * IFPR - Campus Cascavel
 * Disciplina: Programação Orientada a Objetos
 * Professor: Nelson Bellincanta
 * Aluna: Heloísa Raquel Siebeneichler
 */

public class Pessoa{//criação da classe "Pessoa"
  
  private String nome;//criação do atributo string 'nome'
  private int idade;//criação do atributo inteiro 'idade'
  private double altura;//criação do atributo double 'altura'


  //criação do método para retornar a string nome 
  public String getNome(){
    return nome;
  }
   //criação do método para retornar o int idade 
  public int getIdade() {
    return idade;
  }
  //criação do método para retornar o double altura 
  public double getAltura() {
    return altura;
  }
  //metodo para setar o nome
  public void setNome(String nome) {
    this.nome = nome;
  }
    //metodo para setar a idade
  public void setIdade(int idade) {
    this.idade = idade;
  }
    //metodo para setar a altura
  public void setAltura(double altura) {
    this.altura = altura;
  }
}

  ```
