
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
