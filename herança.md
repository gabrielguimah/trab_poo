Exemplo de Herança:

```java
public class Pessoa {
  public String nome;
  public double idade;
  public double cpf;
}
  
public class Aluno extends Pessoa {
  public double matricula;
  public double media;
}
    
public class Professor extends Pessoa {
  public double salario;
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
