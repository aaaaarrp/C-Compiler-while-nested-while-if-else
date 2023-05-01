# C/C++ Compiler for while loop with nested while loop and/or if-else constructs.

Simulation of the front-end and back-end phase of a C compiler involving the If-Else, While and nested If-Else-While constructs.</br>
This includes SIX phases of a compiler:</br>
1) Lexical Analysis- Entering into an Input Table.</br>
2) Syntactic Analysis- Creation of an Abstract Syntax Tree.</br>
3) Semantic Analysis- Verifying Type compatability and generating the Intermediate Code.</br>
4) Intermediate Code Generation - Three Address code generated in Quadruples</br>
5) Machine Independent Code Optimization - Constant Folding, Common Sub-Expression Elimination, Dead Code Elimination<br>
6) Assembly Code Generation - Final Target Code<br>

To Run the compiler, clone the github repo -
> git clone https://github.com/aaaaarrp/C-Compiler-while-nested-while-if-else.git

Then run the script `compile.sh` -
> ./compile.sh 

Few informations about the files -
- lexer.l is the lexical analyzer which is written in lex.
- parser.y runs parser which is written in YACC.
- y.tab.h and y.output (debugger for parser).
- GenInput.txt - Parser generated Quadruples INPUT to generate Assembly Language.
- OpInput.txt - Three address code INPUT for Code optimization.
- Python scripts are used for Code optimization and Assembly code generation from quadruples.