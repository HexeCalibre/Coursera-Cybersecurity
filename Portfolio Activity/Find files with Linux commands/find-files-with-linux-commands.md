# Activity: Find files with Linux commands

## Activity overview
Previously, you learned about Linux and how to communicate with the OS through the shell. You also learned how to use some of the core commands to navigate the Linux file system and read content from files it contains.

These are essential skills. For example, when investigating unauthorized access, you might navigate to and then read a user access report.

In this lab activity, you’ll navigate a Linux file structure, locate files, and read the contents of files. You’ll also need to answer a few multiple-choice questions based on the information contained in these files.

As a security analyst, it’s key that you know how to navigate, manage, and analyze files remotely via a Linux shell without a graphical user interface.

## Scenario
In this scenario, you have to locate and analyze the information of certain files located in the `/home/analyst` directory.

Here’s how you’ll do this: **First**, you’ll get the information of the current working directory you’re in and display the contents of the directory. **Second**, you’ll navigate to the `reports` directory and list the subdirectories it contains. **Third**, you’ll navigate to the `users` subdirectory and display the contents of the `Q1_added_users.txt` file. **Finally**, you’ll navigate to the `logs` directory and display the first 10 lines of a file it contains.

To complete these tasks, you'll need to use commands that you've previously learned in this course. Well, it's time to practice what you’ve learned. Let’s do this!

## Task 1. Get the current directory information
In this task, you must use the commands you learned about to check the current working directory and list its contents.

1. Display your working directory.
2. Display the names of the files and directories in the current working directory.

## Task 2. Change directory and list the subdirectories
In this task, you must navigate to a new directory and determine the subdirectories it contains.

1. Navigate to the `/home/analyst/reports` directory.
2. Display the files and subdirectories in the `/home/analyst/reports` directory.

## Task 3. Locate and read the contents of a file
In this task, you must navigate to a subdirectory and read the contents of a file it contains.

1. Navigate to the `/home/analyst/reports/users` directory.
2. List the files in the current directory.
3. Display the contents of the `Q1_added_users.txt` file.

## Task 4. Navigate to a directory and locate a file
In this task, you must navigate to a new directory, locate a file, and examine the contents of the file.

1. avigate to the `/home/analyst/logs` directory.
2. Display the name of the file it contains.
3. Display the first **10** lines of this file.

## Conclusion
Great work!

You now have practical experience in using basic Linux Bash shell commands to

- navigate directory structures with the cd command,
- display the current working directory with the pwd command,
- list the contents of a directory with the ls command, and
- display the contents of files with the cat and head commands.

Navigating through directories and reading file contents are fundamental skills that you’ll often use when communicating through the shell.