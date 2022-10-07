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
  
public class Pinguim extends Animal  {
  public String especie;
}
    
public class Gaivota extends Animal implements Voador {
  public String especie;
      
  @Override
  public void voar() {
    System.out.println("A espécie está voando!");
  }
}
```
