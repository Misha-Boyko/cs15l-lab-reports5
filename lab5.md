# Lab 5
## Here is the theoretical EdPost that would be posted by a student:

## What environment are you using (computer, operating system, web browser, terminal/editor, and so on)?
I am using a Laptop LG Gram which operates on Windows 11. I am using the VSCode editor with java 17.0.5 2022-10-18 LTS.


## Detail the symptom you're seeing. Be specific; include both what you're seeing and what you expected to see instead. Screenshots are great, copy-pasted terminal output is also great. Avoid saying “it doesn't work”.
When I type the command ```bash runB.sh``` which should run the bash script, the terminal crashes. All I have in the bash script is the compile and running of a java file I've called "HelloWorld". The java file 
prints "Hello World" perfectly to the terminal when I run the compiling and running commands seperately, but when I try and use the bash script, the terminals crashes. 
![Image](termBash.png.png)
![Image](helloW.png.png)

## Detail the failure-inducing input and context. That might mean any or all of the command you're running, a test case, command-line arguments, working directory, even the last few commands you ran. Do your best to provide as much context as you can.
I'm in the PS C:\Users\mboyk\CSE15L\DemoLab5> working directory which houses the HelloWorld.java and the runB.sh script. I run the bash script in the working directory, and it fails. I tried
running the bash script before and after manually compiling the java file, but in either case the terminal crashes.
Thanks for any help!
Misha

# 1. TA Response:
Hello Misha, 
I'm looking at your terminal, and I noticed that although it says "bash" on the right side of the terminal screen, your working directory is given in similar form to that of the powershell
format for Windows. Could you try and press the down arrow next to the "+" on the right side of your terminal and add a "Git Bash" terminal. From there try running the same bash command as before ```bash runB.sh``` and 
let me know if it's still freezing your terminal. Thanks for the detailed description of your bug, hope this helps!

# 2. 
That fixed it!
![Image](successB.png)
The bug was that although the student believed they were running their bash commands in a bash terminal, in reality, the terminal trying to run the commands was not appropriate. The powershell terminal initally says "powershell" on the right side of the terminal when added, but after typing a bash command into the terminal, it becomes called "bash" which can be confusing and has confused me in the past. I decided to choose this bug because it has happened to me in the past and the help from google on this particular bug is difficult to find.

