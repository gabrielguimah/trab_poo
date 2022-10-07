Exemplo de Herança:

```java
public class Pessoa {
  public String nome;
  public double idade;
  public double cpf;
}
  
public class Aluno extends Pessoa {
  public double matricula;
  public String media;
}
    
public class Professor extends Pessoa {
  public double salario;
}
```

Exemplo de Implementação de Interface:

```java
public class Animal {
  public String filo;
  public double classe;
  public double ordem;
  public double familia;
  public double genero;
}

public interface Voador {
  void voar()
}

public interface NaoVoador {
  void caminhar()
}
  
public class Pinguim extends Animal implements NaoVoador {
  @Override
  public void caminhar() {
    System.out.println("A espécie está caminhando!");
  }
}
    
public class Gaivota extends Animal implements Voador {
  @Override
  public void voar() {
    System.out.println("A espécie está voando!");
  }
}
```
