# Flower Language Translator

## Project Description
The Flower Language Translator is a task-oriented programming language designed for grid-based agent navigation. This project was developed as part of the Languages and Compilers (CSC 3315) course.

Key features:
- Custom grammar inspired by C for basic command compilation
- Lexer and parser implementation
- Intermediate code generation (tokens and Abstract Syntax Tree)
- Functional interpreter for executing machine code

## Project Structure
- `flwr_lexer.py`: Lexical analyzer for the Flower language
- `flwr_parser.py`: Parser for the Flower language (generates AST and CST)
- `main.py`: Main script to run the lexer and parser
- `interpreter.c`: Interpreter for executing machine code
- `test_suit/`: Directory containing sample Flower language programs
  - `test1.flwr`, `test2.flwr`, ...: Example Flower language code files

## How to Run
1. Ensure you have Python installed on your system.
2. Clone this repository:
   ```
   git clone https://github.com/yourusername/FlowerLanguageTranslator.git
   cd FlowerLanguageTranslator
   ```
3. Run the main script to process Flower language files:
   ```
   python main.py
   ```
   This will process all `.flwr` files in the `test_suit` directory.

4. To run the interpreter:
   ```
   gcc interpreter.c -o interpreter
   ./interpreter
   ```
   Note: You'll need to provide appropriate input for the interpreter based on your Flower language program.

## Compilation Process
1. The lexer (`flwr_lexer.py`) analyzes the input Flower language code and generates tokens.
2. The parser (`flwr_parser.py`) takes these tokens and constructs the Abstract Syntax Tree (AST) and Concrete Syntax Tree (CST).
3. (Not implemented) The next step would be to generate machine code from the CST.
4. The interpreter (`interpreter.c`) is implemented and can execute machine code once it's generated.

## Note
The step from CST to machine code generation is not implemented in this version. However, the interpreter (`interpreter.c`) is fully functional and can execute machine code. To complete the compilation process, future development should focus on implementing the machine code generation step from the CST.
