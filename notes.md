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

thing=\$(uname -a)

This is the format to assign the value of the result of what is in the parenthesis to the variable thing.

**File Permission**

You need to make the ex file:

- you can first check the file permission with ls -l
- To make it executable you can do chmod +x over the file
- we can make the script without the extension

**Loops**

for thing in list of things; do
done

- we can check the syntax by using bash -n script + echo \$?

**Inputs**

- From the user: read -p 'prompt' var
You can enve pipe it

**If statements**

if ....; then
if [[ -n $1 ]]; then
    name=$1
else
    read -p 'enter your name: ' name
fi


- for loops we can use \$@ to take args as long as we give them to the program.

 ### Functions


true returns 0 etc.


**Inputs**

%> write a file
%> pass to a file


\$# is the sum ofhte arguments given

>&2 we are redirecting to the file descriptor 2

exit 1 breaks the script + code 1

d*= check name starts with d


Shift move the array of arguments by one 
