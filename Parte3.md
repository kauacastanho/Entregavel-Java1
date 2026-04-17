# Entregável Java 01 


## Parte 3 - Paradigma de Programação Orientado a Objetos (POO)

### O que é POO

A Programação Orientada a Objetos (POO) é um paradigma de programação baseado na organização do código em objetos, que representam entidades do mundo real. Esse modelo facilita a reutilização, organização e manutenção do código.

---

### 1. Classe
Uma classe é como um molde ou modelo para criar objetos. Ela define atributos (variáveis) e métodos (funções).

```java
class Pessoa {
    String nome;
    int idade;

    void apresentar() {
        System.out.println("Olá, meu nome é " + nome);
    }
}
```

---

### 2. Objeto
Um objeto é uma instância de uma classe, ou seja, é a representação concreta daquela classe.

```java
public class Main {
    public static void main(String[] args) {
        Pessoa p1 = new Pessoa();
        p1.nome = "João";
        p1.idade = 20;

        p1.apresentar();
    }
}
```

---

### 3. Encapsulamento
Encapsulamento é o conceito de proteger os dados, permitindo acesso apenas por métodos específicos (getters e setters).

```java
class Conta {
    private double saldo;

    public double getSaldo() {
        return saldo;
    }

    public void depositar(double valor) {
        saldo += valor;
    }
}
```
Aqui, o atributo saldo não pode ser acessado diretamente.

---

### 4. Herança
Herança permite que uma classe herde características de outra, promovendo reutilização de código.

```java
class Animal {
    void fazerSom() {
        System.out.println("Som genérico");
    }
}

class Cachorro extends Animal {
    void latir() {
        System.out.println("Au au");
    }
}
```

---

### 5. Polimorfismo
Polimorfismo permite que um método tenha diferentes comportamentos dependendo do contexto.

```java
class Animal {
    void fazerSom() {
        System.out.println("Som genérico");
    }
}

class Gato extends Animal {
    @Override
    void fazerSom() {
        System.out.println("Miau");
    }
}

public class Main {
    public static void main(String[] args) {
        Animal a = new Gato();
        a.fazerSom(); // Executa o método do Gato
    }
}
```

***

A POO é fundamental no desenvolvimento em Java, pois permite criar sistemas mais organizados, reutilizáveis e fáceis de manter. Os conceitos de classe, objeto, encapsulamento, herança e polimorfismo são a base para a construção de aplicações modernas.















