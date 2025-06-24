
# 📘 Resumo das Anotações - Java com Alura
**Curso:** Java: Criando a sua primeira aplicação

---

## ✅ 1. Instalação do JDK
- Instalado o **JDK 21**, versão mais recente com suporte de longo prazo (LTS).
- Link: [Oracle JDK 21 para Windows](https://www.oracle.com/br/java/technologies/downloads/#jdk21-windows)

---

## ⚙️ 2. Configuração da PATH do Java
- Variável de ambiente `Path` configurada com o caminho:
  ```
  C:\Program Files\Java\jdk-21\bin
  ```
- Permite rodar `java` e `javac` de qualquer lugar no terminal.

---

## 💻 3. Instalação do IntelliJ IDEA
- IntelliJ instalado com **todos os checkboxes selecionados**:
  - Atalho na área de trabalho
  - Associação com arquivos `.java`
  - Adição ao menu de contexto
  - Inclusão no `PATH`
  - Plugins recomendados

---

## 🔄 4. Fluxo de Compilação e Execução
- Arquivo `.java` é criado com o código-fonte
- `javac` compila e gera um arquivo `.class` com bytecode
- **JVM** executa o bytecode adaptando-se ao sistema operacional

---

## 📚 5. Conceitos Fundamentais

### 🧠 JVM, JRE e JDK
- **JVM (Java Virtual Machine)**: Executa o bytecode Java.
- **JRE (Java Runtime Environment)**: Contém a JVM e bibliotecas padrão, usadas na execução.
- **JDK (Java Development Kit)**: Contém o compilador, JRE e ferramentas para desenvolvimento.

### 🔢 Tipos Primitivos
- **Inteiros**: `byte`, `short`, `int`, `long`
- **Decimais**: `float`, `double`
- **Caracteres**: `char`
- **Booleanos**: `boolean`

---

## ✍️ 6. Convenções de Código em Java

- **Variáveis e métodos**:
  - Começam com letra **minúscula** (ex: `nomeCompleto`)
  - Estilo *camelCase*

- **Classes**:
  - Começam com letra **maiúscula** (ex: `ClienteVip`)
  - Também usam *camelCase*

- **Constantes**:
  - Escritas em **CAIXA_ALTA** com `_` (ex: `TAXA_DE_IMPOSTO`)

> 🧠 **Motivo**: Aumentar legibilidade, facilitar manutenção e manter padrão profissional.

---

## ➕ Operadores Aritméticos

| Operador | Descrição         | Exemplo     | Resultado |
|----------|-------------------|-------------|-----------|
| `+`      | Adição            | `3 + 2`     | `5`       |
| `-`      | Subtração         | `5 - 3`     | `2`       |
| `*`      | Multiplicação     | `4 * 2`     | `8`       |
| `/`      | Divisão           | `10 / 2`    | `5`       |
| `%`      | Resto da divisão  | `10 % 3`    | `1`       |

---

## ⚖️ Operadores Relacionais

| Operador | Descrição         | Exemplo     | Resultado |
|----------|-------------------|-------------|-----------|
| `==`     | Igual a           | `5 == 5`    | `true`    |
| `!=`     | Diferente de      | `5 != 3`    | `true`    |
| `>`      | Maior que         | `7 > 5`     | `true`    |
| `>=`     | Maior ou igual a  | `5 >= 5`    | `true`    |
| `<`      | Menor que         | `3 < 5`     | `true`    |
| `<=`     | Menor ou igual a  | `3 <= 3`    | `true`    |

---

## 🔗 Operadores Lógicos

| Operador | Nome  | Descrição                                      | Exemplo           | Resultado |
|----------|-------|------------------------------------------------|-------------------|-----------|
| `&&`     | AND   | Verdadeiro se **ambos** forem `true`          | `true && false`   | `false`   |
| `||`     | OR    | Verdadeiro se **um ou ambos** forem `true`    | `true || false`   | `true`    |
| `!`      | NOT   | Inverte o valor lógico                        | `!true`           | `false`   |

---

## 🔼 Operadores de Incremento

| Tipo            | Sintaxe         | Descrição                         | Exemplo         |
|-----------------|------------------|-------------------------------------|-----------------|
| Pré-incremento  | `++variavel`     | Incrementa antes de usar o valor   | `int x = ++a;`  |
| Pós-incremento  | `variavel++`     | Usa o valor e depois incrementa    | `int x = a++;`  |

#### Exemplo prático:
```java
int a = 5;
int b = ++a; // b = 6, a = 6
int c = a++; // c = 6, a = 7
```

---

## ✍️ String é uma classe!

 - Em Java, String não é um tipo primitivo, mas sim uma classe da biblioteca padrão (java.lang.String).
 - Apesar disso, ela pode ser usada como se fosse um tipo básico, pois a linguagem trata String de forma especial (por exemplo, com o uso direto de aspas duplas).

📌 Exemplo:

```java
String nome = "Guilherme";
System.out.println(nome.toUpperCase()); // Exibe: GUILHERME
```

🔍 Características:

  - Strings são imutáveis: uma vez criada, não pode ser modificada (qualquer operação cria uma nova String).

  - Possui vários métodos úteis, como: <b>length(), toUpperCase(), toLowerCase(), contains(), substring(), etc. </b>

É possível criar uma String com:

```java
String texto = new String("Olá");
```
- Internamente, String é tratada como uma sequência de caracteres (char[]).


## 🔍 Comparação de Strings em Java

- O operador == não compara o conteúdo das strings, apenas verifica se as duas variáveis apontam para o mesmo objeto na memória.
- Para comparar o conteúdo textual de duas strings, use o método .equals().

Exemplo:

````java
String s1 = "Java";
String s2 = "Java";
String s3 = new String("Java");

System.out.println(s1 == s2);       // true (mesmo objeto por causa do pool de strings)
System.out.println(s1 == s3);       // false (objetos diferentes)
System.out.println(s1.equals(s3));  // true (conteúdo igual)
````


## 📝 Text Block em Java (Introduzido no Java 15)

- Text Block é uma forma simplificada de criar Strings multilinha.
- Facilita a escrita de textos longos, com quebras de linha e formatação preservadas, sem precisar usar concatenações ou caracteres especiais.
- Utiliza três aspas duplas (""") para delimitar o texto.

Exemplo:
````java
String json = """
{
"nome": "Guilherme",
"idade": 33,
"profissao": "Desenvolvedor"
}
""";
System.out.println(json);
````

## 🖋️ Formatação de Textos em Java com String.format()

- O método format() da classe String permite criar textos formatados utilizando placeholders.
- Placeholders são representados por % seguido de uma letra que indica o tipo de dado.

- Placeholders comuns:
  - <b>%s</b> — String
  - <b>%d</b> — Inteiro decimal
  - <b>%f</b> — Número de ponto flutuante

```java
String nome = "Guilherme";
int idade = 33;
double salario = 2500.75;

String textoFormatado = String.format("Nome: %s, Idade: %d, Salário: %.2f", nome, idade, salario);
System.out.println(textoFormatado);
```
Saída:

````java
Nome: Guilherme, Idade: 33, Salário: 2500.75
````

## 🖋️ Formatação com Text Blocks usando formatted()

- Além do String.format(), a partir do Java 15 é possível usar o método formatted() diretamente em Text Blocks e Strings.
- O método formatted() recebe os valores que substituirão os placeholders (%s, %d, etc.) no texto.

Exemplo com Text Block:

```java
String texto = """
Nome: %s
Idade: %d
Salário: %.2f
""".formatted("Guilherme", 33, 2500.75);

System.out.println(texto);
```
Saída:

```java
Nome: Guilherme
Idade: 33
Salário: 2500.75
```

---
