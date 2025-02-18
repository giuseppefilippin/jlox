# Lox Interpreter in Java

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white)
![Compiler](https://img.shields.io/badge/Compiler-Interpreter-blue)
![Crafting Interpreters](https://img.shields.io/badge/Crafting-Interpreters-yellow)

## 📖 About the Project

This repository contains an implementation of the **Lox** programming language interpreter, written in Java, following the book [Crafting Interpreters](https://craftinginterpreters.com/) by Robert Nystrom. The project is currently in the **Tree-Walk Interpreter** phase, which means it executes the AST directly rather than compiling into bytecode.

## 🛠 Features

- Implements the Lox programming language
- Uses a **recursive descent parser**
- Supports **expressions, variables, functions, and control flow**
- Implements **error handling and reporting**
- Tree-walk execution of AST nodes
- Fully written in **Java**

## 🚀 Getting Started

### Prerequisites

Ensure you have Java installed on your machine:

```sh
java -version
```

If Java is not installed, download and install it from [Adoptium](https://adoptium.net/) or [Oracle](https://www.oracle.com/java/technologies/javase-downloads.html).

### Installation

Clone the repository:

```sh
git clone https://github.com/giuseppefilippin/jlox.git
cd JLOX
```

### Running the Interpreter

Compile and run the Lox interpreter:

```sh
javac -d bin src/com/lox/*.java
java -cp bin com.lox.Lox
```

### Running a Lox Script

You can execute a Lox script by passing a file as an argument:

```sh
java -cp bin com.lox.Lox script.lox
```

### Running in Interactive Mode (REPL)

Run the interpreter without arguments to enter interactive mode:

```sh
java -cp bin com.lox.Lox
```

Example interaction:

```
> print "Hello, world!";
Hello, world!
> 2 + 2 * 3;
8
```

## 📝 Lox Language Overview

### Variables
```lox
var name = "Lox";
print name;
```

### Functions
```lox
fun greet() {
  print "Hello from Lox!";
}
greet();
```

### Control Flow
```lox
if (3 > 2) {
  print "Yes!";
} else {
  print "No!";
}
```

## 🔍 Roadmap

- [x] Scanner (Lexical Analysis)
- [x] Parser (Syntactic Analysis)
- [x] Abstract Syntax Tree (AST)
- [x] Tree-Walk Interpreter
- [ ] Bytecode Virtual Machine (Next Phase)
- [ ] Optimizations & Enhancements

## 📚 References

- **[Crafting Interpreters](https://craftinginterpreters.com/)** by Robert Nystrom
- Java Official Documentation: [https://docs.oracle.com/en/java/](https://docs.oracle.com/en/java/)

## ⭐ Acknowledgments

Special thanks to Robert Nystrom for writing *Crafting Interpreters* and making compiler construction more accessible!

