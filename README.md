# Flower Language Translator

## Project Description
The Flower Language Translator is a task-oriented programming language designed for grid-based agent navigation. This project was developed as part of the Languages and Compilers (CSC 3315) course.

Key features:
- Custom grammar inspired by C for basic command compilation
- Lexer and parser implementation
- Intermediate code generation (tokens and Abstract Syntax Tree)

## Project Structure
- `flwr_lexer.py`: Lexical analyzer for the Flower language
- `flwr_parser.py`: Parser for the Flower language (generates AST and CST)
- `main.py`: Main script to run the lexer and parser
- `interpreter.c`: (Placeholder) Interpreter for executing machine code
- `test_suit/`: Directory containing sample Flower language programs
  - `test1.flwr`, `test2.flwr`, ...: Example Flower language code files

## How to Run
1. Ensure you have Python installed on your system.
2. Clone this repository:
   ```
   git clone https://github.com/yourusername/FlowerLanguageTranslator.git
   cd FlowerLanguageTranslator
   ```
3. Run the main script:
   ```
   python main.py
   ```
   This will process all `.flwr` files in the `test_suit` directory.

## Compilation Process
1. The lexer (`flwr_lexer.py`) analyzes the input Flower language code and generates tokens.
2. The parser (`flwr_parser.py`) takes these tokens and constructs the Abstract Syntax Tree (AST) and Concrete Syntax Tree (CST).
3. (Not implemented) The next step would be to generate machine code from the CST.
4. (Placeholder) The `interpreter.c` file is intended to execute the generated machine code.

## Note
The step from CST to machine code generation is not implemented in this version. The interpreter (`interpreter.c`) is a placeholder for future development to execute the compiled Flower language programs.
