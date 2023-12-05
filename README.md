# trabalho_oo

// Pessoa.java

public class Pessoa {
  
    private String nome;
    private int idade;
    private String numeroTelefone;


    public Pessoa(String nome, int idade, String numeroTelefone) {
        this.nome = nome;
        this.idade = idade;
        this.numeroTelefone = numeroTelefone;
    }

    public String getNome() {
        return nome;
    }

    public void setNome(String nome) {
        this.nome = nome;
    }

    public int getIdade() {
        return idade;
    }

    public void setIdade(int idade) {
        this.idade = idade;
    }

    public String getNumeroTelefone() {
        return numeroTelefone;
    }

    public void setNumeroTelefone(String numeroTelefone) {
        this.numeroTelefone = numeroTelefone;
    }

  
    public void imprimirInformacoes() {
        System.out.println("Nome: " + nome);
        System.out.println("Idade: " + idade);
        System.out.println("Número de Telefone: " + numeroTelefone);
    }

   
    public static void main(String[] args) {
     
        Pessoa pessoa = new Pessoa("João", 25, "123-456-7890");

        
        System.out.println("Nome antes da modificação: " + pessoa.getNome());
        pessoa.setNome("Maria");
        System.out.println("Nome depois da modificação: " + pessoa.getNome());

        pessoa.imprimirInformacoes();
    }
}
