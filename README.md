# Compiler-Construction-Lexical-analyzer
### Implemented Features
1. **Lexical Analyzer**:
   - Tokenization of source code into identifiers, keywords, numbers, operators, braces, semicolons, strings, and character literals.
   - Handling of single and multi-line comments effectively.
   - Management of whitespace and newlines, incrementing line count appropriately for error reporting.
   - Error handling for unrecognized tokens and malformed literals.

2. **Regular Expressions, NFA, and DFA**:
   - Custom regular expressions for identifiers, numbers, and operators.
   - NFAs and DFAs with transitions that manage the identification process for different types of tokens.

3. **Symbol Table**:
   - Dynamic management of scopes with global and local context awareness.
   - Recording identifiers along with their data types and scopes.

4. **Error Handling**:
   - Reporting of lexical errors with specific line numbers and error descriptions.
   - Identification of unclosed comments, string literals, and character literals.

### Language Specifications
- **Keywords**: `int`, `decimal`, `bool`, `char`, `string`, `true`, `false`
- **Data Types**:
  - **Boolean**: For true/false values.
  - **Integer**: For whole numbers.
  - **Decimal**: For decimal numbers, accurate up to five places.
  - **Character**: For single letters.
- **Operators**: Includes arithmetic (`+`, `-`, `*`, `/`, `%`) and logical (`<`, `<=`, `>`, `>=`, `==`, `!=`).
- **Comments**: Handles both single-line (`//`) and multi-line (`/* ... */`) comments.
- **Identifiers**: Recognizes sequences starting with letters followed by digits and underscores.

### Setup and Execution
1. **Compilation**:
   - Compile the Java files using `javac Compiler.java`.
2. **Running the Lexer**:
   - Execute `java Compiler` to run the lexer. Ensure the `input.redblack` file path is correctly specified in the source code.
3. **Outputs**:
   - The console will display the tokens, error messages, and the symbol table contents.

### Error Handling
The lexer integrates an error handling mechanism that captures and reports lexical errors, unclosed string or character literals, and improperly formatted numbers.

