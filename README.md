**COMPILER**


**wec_task.c** 
. file contains the handwritten c code for lexer and parser.
. It was done to get the idea of how does a lexer and parser work.
. The user should enter the string as input.
. The function lexer converts the input string into the tokens mentioned in the code.
. The tokens are sent to parser which checks if the tokens are following the grammar mentioned or not.


**wec_taskn.l**
. This file is the lexer code using flex in c .
. The user should give the string as input.
. the input is converted into tokens as mentioned in the code.


**wec_task44.y**
. this file is the parser code using bison i c.
. this takes the tokens from lexer as input.


**wec.c**
.this is the additional c file to connect lexer and parser.

**commands to run the codes**
wec_task.c-handwritten lexer and parser
    gcc wec_task.c
    ./a.out
for lexer and parser using flex and bison
    flex wec_taskn.l
    bison -dy wec_task44.y
    gcc -c lex.yy.c
    gcc -c wec.c
    gcc -c wec_task4.c
    a.exe


**Used concepts(learnt for the task):-**
1.regular expressions.
2.context free grammar
3.working of lexer and parser
4.implementation of lexer using flex
5.implementation of parser using bison
6.abstract syntax tree
