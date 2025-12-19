# Bash Course Notes


## Lecture 1: Introduction to Bash and Terminal Basics


- Bash is a program, shell= REPL-> Read Eval Print Loop
- Bash is always in a folder (pwd) print working directory

### Basic File Manipulation

We can use: rm -i (interactive)

- Ctrl l = clear the screen
- Ctrl-shift-b is backward searching

**Searching Files and Paging**


- grep: program that looks for a pattern in a file
- ^ it has to match the beginning of the line
- $ it has to match the end of the line
- > overwrite the file, >> append to the file
- grep -A1 b file.txt (find b and the line After that), you can use also B for before, C (context)
- grep -o '^d.' file.txt = matches
- grep -i word file.txt it's case insentive
- grep -o only print the part that matches the pattern: only print the part that matches



**Pagers**

- less: it shows the content of the file in a page

**Man pages**

- man gives you the manual for external commands
- --help works for system commands (like history)

## Chapter 02:

**Programs and Commands**


- file text.txt it tells you what kind of file it is 

- tr (translate ) : echo $PATH | tr : "/n"

- "$PATH" is a random variable 

thing=$(uname -a)

This is the format to assign the value of the result of what is in the parenthesis to the variable thing. 


