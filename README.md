# C-Compiler


I have implemented a C compiler using flex and bison as tokenizer and parser. This compiler gets a C language program file as input and provides a MIPS assembly output file.

## Usage guide

### Requirements
* flex
* bison (Konsole is a terminal emulator built on the KDE Platform). See [flex & bison]


* [flex & bison](https://web.iitd.ac.in/~sumeet/flex__bison.pdf)
* [flex & bison](https://aquamentus.com/flex_bison.html)
* (https://www.oreilly.com/library/view/flex-bison/9780596805418/ch01.html)
 
### Step 1: Download Tokenizer.l & Parser.y Files
You can clone codes using the below command:
```
git clone https://github.com/SaraBaradaran/C-Compiler
```

### Step 2: Compile & Run Files
```
flex tokenizer.l
bison -d parser.y
gcc parser.tab.c lex.yy.c -o compiler
```

### Step 3: Modify input.txt File 

You may want to modify input.txt file based on your C program.
consider in this compiler we support these structures :

* int data type
* variable declaration & definition
* function definition (functions having void or int output data type)
* while
* if 
* function call
* array
* global variables
* scope checking 
* 
Finally, run `./script.sh` file.
