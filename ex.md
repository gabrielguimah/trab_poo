Exemplo de Herança:

```java
public class Pessoa {
  private String nome;
  private int idade;
  private int cpf;
}
  
public class Aluno extends Pessoa {
  private int matricula;
  private double media;
  private String turma;
}
    
public class Professor extends Pessoa {
  private double salario;
  private String turma;
}
```


Exemplo de Implementação de Interface:

```java
public class Animal {
  public String filo;
  public String classe;
  public String ordem;
  public String familia;
  public String genero;
}

public interface Voador {
  void voar()
}

public interface NaoVoador {
  void caminhar()
}
  
public class Pinguim extends Animal implements NaoVoador {
  public String especie;
  
  @Override
  public void caminhar() {
    System.out.println("A "+ especie + " está caminhando!");
  }
}
    
public class Gaivota extends Animal implements Voador {
  public String especie;
  
  @Override
  public void voar() {
    System.out.println("A "+ especie + " está voando!");
  }
}
```


Exemplo de Sobrecarga:

```java
public static int calcular(int num){
  int calculo;
  quadrado = num * num * num;
  return calculo;
}

public static double calcular(double num){
  double calculo;
  quadrado = num * num * num;
  return calculo;
}
    
public static void main(String[] args){
  System.out.println("Resultado de 4 elevado ao cubo => " + calcular(4));
  System.out.println("Resultado de PI elevado ao cubo => " + calcular(Math.PI));
}
```

Exemplo de Composição:

```java
public class Time {
  double valor;
  int qtd_jogadores;
  String nome;
  double verba;
  String estadio;
}

public class Jogador {
  double salario;
  String nome;
  double valor;
  boolean titular;
  Time nome
}
```
