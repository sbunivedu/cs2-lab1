# Lab 1 Orientation
## Purpose
The purpose of this lab is to get oriented to writing programs in Java using a command line interface in Linux.  To that end, in this lab we will learn how to:
* Run commands in a Linux command line.
* Use some Linux commands to create directories (folders), rename some files, delete some files, print some files.
* Use `javac` to compile a Java source file
*	Use `java` to run a Java class file
*	Review looping and `if` statements in Java

## Evaluation
Students will be awarded up to 10 points for successfully completing this lab as outlined below.

## Instructions

Step 1. Log into your `cisone.sbuniv.edu` account using `Putty` app on Windows or `Terminal` app on Mac.

Step 2. Experiment with the following Linux commands:

1. Create a directory named `CS2` using `mkdir`, the "Make Directory" command.
```shell
[blu@cisone ~]$ mkdir CS2
```

2. Now "list" your files and directories using the `ls` command.
```shell
[blu@cisone ~]$ ls
```

3. Now, move to the CS2 directory using the "Change Directory" command, `cd`.
```shell
[blu@cisone ~]$ cd CS2/
[blu@cisone CS2]$ 
```
Notice your "prompt" has changed to indicate you have moved to a new directory.  We would call CS2 our current directory.

4. Before you leave the CS2 directory, make a new subdirectory in the CS2 directory called "lab1."

5. Make lab1 your current directory by moving to it with the `cd` command.

Step 3. Create a new file named, of course, `HelloWorld.java` using `nano HelloWorld.java` commands in the `lab1` directory you created earlier.
Write the traditional HelloWorld program shown below:
```java
public class HelloWorld{
  public static void main (String [] args){
    System.out.println("Hello World!");
  }
}
```
Step 4. Running `HelloWorld.java` in Linux.

Start by listing the contents of your `CS2/lab1` directory with the `ls` command. Do you see the `HelloWorld.java` file you created?

To compile your program, you should use the Java compiler called `javac`. The command is shown below:
```shell
[blu@cisone lab1]$ javac HelloWorld.java
```
If everything is OK syntax-wise, you’ll be rewarded with another prompt.  If there are problems, `javac` will try and tell you where they are in the code.  You’ll need to go and fix them before proceeding.

Once your program compiles, `javac` will produce a class file, which can be run.  See if you can find the `.class` file with the list command. Now you are ready to run your program as shown below.
```shell
[blu@cisone lab1]$ java HelloWorld  
Hello World!
```
Step 5. Practice

Now that you know how to write and run a Java program in Linux, you should practice your new-found skill by modifying your HelloWorld program.  Review looping (for, while, do) and selection (if) control structures by creating a different loop to produce each of the following sequences. You should end up with __4 different loops__ in your main method.  Use at least one `for` loop, one `while` loop, and one `do while` loop.
* 987654321
* 2 0 3 0 4 0 5 0 6 0 7
* 4 9 14 19 24
* 111 110 109 108 107 106 105 104

Step 6. Submit your work

Please follow the `git` workflow to commit your code to the git repository for this assignment and push the changes to `github`.
