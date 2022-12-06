Assembler - An assembler enables software and application developers to access, operate and manage a computer's hardware architecture and components.
An assembler is sometimes reffered to as the compiler of assembly language. It also provides the services of an interpreter. Assemblers are classified based on the number of times it takes them to read the source code before translating it. 

There are two different types of assemblers
1. one-pass assembler 
2. two-pass assembler
 
1. one-pass assembler : scans the program only once and creates the equivalent binary program, the assembler substitute all of the symbolic instruction with machine code in one pass. In first pass it collect the symbols and labels and assembles the instruction ( e.g. [MASM](https://en.wikipedia.org/wiki/Microsoft_Macro_Assembler)) 

2. two-pass assembler : in first pass it collects the labels and symbols and in second pass it assembles the instructions, it stores mnemonics and pseudo codes separately, literals and symbols are stored in literal and symbol table respectively, the second pass assembler locates and completes (using the symbol table) the partial instruction (e.g. [JWASM](https://en.wikipedia.org/wiki/Open_Watcom_Assembler))

Why 2 pass assembler?
One pass assembler cannot resolve forward references of data symbols. It requires all data symbols to be defined prior to being used. A two-pass assembler solves this dilemma by devoting one-pass to exclusively resolve all (data/label) forward references and then generate machine code with no hashels in the next pass![assembly_diagram](https://user-images.githubusercontent.com/72422013/116241199-44652b00-a782-11eb-814f-b4e43aa6b94b.png)
<img width="636" alt="flow_char_2pass" src="https://user-images.githubusercontent.com/72422013/116241220-48914880-a782-11eb-98d5-f6f5cd4dc41f.png">
