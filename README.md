📘 Lexical Analyzer in C

A simple and efficient Lexical Analyzer (Lexer) implemented in the C programming language.
This project scans a C source file, identifies tokens, categorizes them, and reports lexical errors.

🚀 Features
Detects Keywords
Identifies Identifiers
Recognizes Operators
Handles Delimiters
Supports:
Decimal Numbers
Hexadecimal Numbers
Octal Numbers
Binary Numbers
Floating Point Numbers
Processes:
String Literals
Character Literals
Detects lexical errors such as:
Invalid identifiers
Invalid operators
Unterminated strings
Invalid constants
Unmatched delimiters
📂 Project Structure
├── main.c              # Main driver program
├── lexer.h             # Header file with declarations
├── keywords.c          # Keyword and identifier handling
├── operators.c         # Operator handling
├── delimeters.c        # Delimiter processing
├── digit.c             # Numeric literal handling
├── literals.c          # String and character literal handling
├── file.txt            # Input C source file
├── Documentation.txt   # Project documentation
⚙️ Technologies Used
Language: C
Compiler: GCC
IDE: VS Code / CodeBlocks
🛠️ How It Works
Reads the input source file character by character.
Classifies tokens into categories.
Prints recognized tokens.
Reports lexical errors with line and column numbers.
▶️ Compilation & Execution
Compile
gcc main.c keywords.c operators.c delimeters.c digit.c literals.c -o lexer
Run
./lexer
🧪 Sample Tokens Detected
int num = 10;

Output:

Keyword : int
Identifier : num
Operators : =
Decimal Number : 10
Delimiter : ;
❌ Error Detection Examples

The lexer can detect:

0x12KAF      // Invalid hexadecimal
0b12011      // Invalid binary
'XY'         // Invalid character literal
printf("Hi)  // Unterminated string
📌 Concepts Covered
Compiler Design
Lexical Analysis
Tokenization
File Handling in C
Error Handling
String Processing
📈 Future Enhancements
Symbol Table Generation
DFA Visualization
Syntax Analyzer Integration
GUI-based Token Viewer
Comment Handling
👨‍💻 Author

N Vamsi Krishna
