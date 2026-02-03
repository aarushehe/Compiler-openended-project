# CompilerOE - A Fun Compiler Project

I built this compiler from scratch just for fun! It's a simple yet complete compiler that takes source code and transforms it through various stages of compilation. This project was my playground to understand how compilers work under the hood.

## What It Does

This compiler processes C-like code through the complete compilation pipeline:
1. **Lexical Analysis** - Breaks code into tokens
2. **Parsing** - Builds syntax trees from tokens
3. **Semantic Analysis** - Checks for errors and builds symbol tables
4. **Code Generation** - Produces intermediate and final code
5. **Optimization** - Makes the generated code better

## Features

### Core Components
* **Clexer** - Tokenizer that reads source code and identifies keywords, identifiers, operators
* **ASTBuilder** - Creates Abstract Syntax Trees from parsed tokens
* **SemanticAnalyzer** - Type checking and scope management
* **ThreeAddressCodeGenerator** - Produces intermediate 3-address code
* **CodeOptimizer** - Simple optimizations like constant folding
* **CodeGeneratorWithRegisterAllocation** - Final code generation

### Output Files
* **OutputLexer** - Shows all the tokens found
* **OutputParser** - Displays the parse tree structure
* **OutputThreeCode** - Intermediate 3-address code
* **OutputCodeOptimize** - Optimized code after processing
* **FinalOutput** - The final compiled result

## How to Use

1. **Compile the compiler**:
   ```
   javac *.java
   ```

2. **Run it on a C-like file**:
   ```
   java Main yourfile.c
   ```

3. **Check the outputs**:
   * Look in the `outputs/` folder for final results
   * Check `input/` folder for intermediate step outputs

## Files in This Project

### Source Files
* `ASTBuilder.java` - Builds syntax trees
* `Clexer.java` - Tokenizer for C-like syntax
* `SemanticAnalyzer.java` - Checks for semantic errors
* `ThreeAddressCodeGenerator.java` - Creates intermediate code
* `CodeOptimizer.java` - Optimizes the generated code
* `CodeGeneratorWithRegisterAllocation.java` - Final code output

### Output Files Generated
* `FinalOutput` - The end result
* `FinalAnswer` - Summary of compilation
* Various intermediate files showing each compilation step

## Try It Yourself

```
# Compile the compiler
javac *.java

# Run on a test file
java Main test.c

# See what happens at each step!
cat input/OutputLexer
cat input/OutputParser
cat outputs/FinalOutput
```

## Note

This is a **learning project** - it's not production-ready! It handles basic C-like syntax and was built for educational purposes. If you find bugs, that's part of the fun! Feel free to fork it and make it better.

---

*Built with curiosity and a lot of coffee ☕*
