This is a project of 2 pass assembler 
Manual and other documentation will be updated soon
1. Program in C
2. Python conversion and further improvemnet
3. React implementaion (future scope) - UI for interactiveness

Assembler - An assembler is a type of computer program that iterprets software programs written in assembly language into machine language, code and instruction that can be executed by a computer. 

An assembler enables software and application developers to access, operate and manage a computer's hardware architecture and components.
An assembler is sometimes refferd to as the compiler of assembly language. It also provides the services of an interpreter. Assemblers are classified based on the number of times it takes them to read the source code before translating it. 

There are two different types of assemblers
1. one-pass assembler 
2. two-pass assembler
 
1. one-pass assembler : scans the program only once and creates the equivalent binary program, the assembler substitute all of the symbolic instruction with machine code in one pass. In first pass it collect the symbols and labels and assembles the instruction ( e.g. (MASM)[https://en.wikipedia.org/wiki/Microsoft_Macro_Assembler]) 

2. two-pass assembler : in first pass it collects the labels and symbols and in second pass it assembles the instructions, it stores mnemonics and pseudo codes seperately, literals and symbols are stored in literal and symbol table respectively, the second pass assembler locates and cpmpletes (using the symbol table) the partial instruction (e.g. (JWASM)[https://en.wikipedia.org/wiki/Open_Watcom_Assembler])

![Diagram](ihttps://github.com/sayantan3/assembler/blob/MAIN/assembly_diagram.png?raw=true)

Why 2 pass assembler?
One pass assembler cannot resolve
