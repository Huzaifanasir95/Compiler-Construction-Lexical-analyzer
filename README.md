# Compiler-Construction-Lexical-analyzer

### File Structure
- **Compiler.java**: Contains the main class implementing the lexical analyzer.
- **input.redblack**: Sample input file with code written in the custom language.

### Language Constructs
Our language supports various constructs which are categorized into identifiers, numbers, operators, and keywords. The analyzer breaks input into tokens, each classified into one of the following types:
- **Keywords**: Reserved words with special meaning in the language.
- **Identifiers**: Names used to identify entities like variables and functions.
- **Numbers**: Integer or floating-point literals.
- **Operators**: Symbols representing operations like addition, subtraction, etc.
- **Braces**: Used for defining scopes.
- **Semicolons**: Statement terminators.

### Keywords
The following are reserved keywords in the language:
- `if`, `else`, `while`, `for`
- `int`, `decimal`, `bool`, `char`, `string`
- `true`, `false`

### Regular Expressions
The analyzer uses these regular expressions for tokenizing:
- **Identifiers**: `[a-z]+[a-z0-9_]*`
- **Numbers**: `digit+ ('.' digit{1,5})? ([Ee][+-]? digit+)?`
- **Operators**: `[+\\-*/%<>=!]|==|<=|>=|!=`

### Usage
To use the lexer, follow these steps:
1. **Setup Environment**: Ensure Java is installed and setup correctly on your system.
2. **Compile the Java Code**: Use the Java compiler to compile the `Compiler.java`.
3. **Run the Analyzer**: Run the compiled code. Make sure to provide the path to the `input.redblack` file when prompted or modify the code to automatically read this file.
4. **Review Output**: The output will display tokens identified by the lexer, any errors encountered, and the symbol table contents.

### Error Handling
The lexer incorporates comprehensive error handling to manage:
- **Syntax Errors**: Incorrect use of the language syntax.
- **Semantic Errors**: Errors related to the meaning of the constructs, like using undeclared variables.

### Output
Outputs from the lexer include:
- **Token List**: Each token detected in the input file.
- **Errors**: Any errors detected during the lexical analysis.
- **Symbol Table**: Shows all symbols identified and their scopes.

### Conclusion
This lexical analyzer is designed to be robust and user-friendly, providing clear error messages and detailed token information, which are crucial for debugging and understanding the structure of programs written in the custom language.
