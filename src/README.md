Project 1: Tokenizer
====================
# Instructions:

There are three main C files that make up the program.

1) History.c
    This file contains all methods pertaining to the query of the history list in the project. 
    It utilizes a linked list in order to save every sentence to a node, and an ID to find that node. 

2) Tokenizer.c
    This file contains all methods pertaining to the tokenizing of the sentences inputed by the user. 
    The UI will call on this functions in order to toekenize words in a sentence by the user. 
    This file is executed by the UI itself just like history.c. 

3) UI.c
    This file was custom made by me, it was suggested to make a UI file in order to read the input of a user and be able to print results from the tokenizer. The UI file will execute commands in the History.c and the Tokenizer.c to execute the whole program fully. The UI is in charge of receiving and outputting data taken from the user. It gives the user a guide to navigate the program.

4) Makefile
    This file when called in the virtual machine command prompt will generate an executable file called "Program" that will boot the UI for the tokenizer. To generate this file, one will have to execute the command "make", in the virtual machine. To remove all files generated by the makefile one will have to execute the command "clean" including the executable. 

4) Program Navigation

    In virtual machine:
        make: Will generate tokenizer executable.
        program: will execute the program.

    Once in the tokenizer program:
        /e: will exit the program.
        /t: will enter tokenize mode.
        /h: will print tokenizer commnads (HELP).
        any input: will be echoed.

        once in /t (Tokenizer mode):
            Enter any sentence in order to tokenize words in sentence.
            Tokenized words will be printed. 
            /l#: Will print the history of the tokenized sentences the user has inputed
                NOTE: replace '#' with any number to look for that enumbered list sentence.
            /e: will exit the program.
