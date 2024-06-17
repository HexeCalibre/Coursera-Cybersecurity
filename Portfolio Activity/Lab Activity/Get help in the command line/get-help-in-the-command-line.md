# Activity: Get help in the command line

## Introduction
In this lab, you’ll use the `man`, `whatis`, and `apropos` commands to practice finding answers to Linux questions in the command line. These skills are useful for many different security tasks. You’ll use Linux commands in the Bash shell to complete this lab.

## Activity overview
As a security analyst, you won’t have all the answers all the time, but you can learn where to find them. One of the great things about Linux is that you can get help right through the command line.

In this lab activity, you’ll use the `man` and `whatis` commands to get information on other commands and how they work. You’ll also use the `apropos` command to search the manual page for a command with a specified string.

When working as a security analyst, you'll likely find it useful to know how to discover which command to use or information about what commands do.

With that in mind, let’s explore your scenario.

## Scenario
In this scenario, you have to find more information about commands that you need to use. You also need to discover which command to use to perform a certain task.

Here’s how you’ll do this task: **First**, you’ll explore a few commands you can use in the shell to learn more about other commands. **Next**, you’ll find an option you need to add to a command. **Third**, you’ll use a command to get a brief description of commands so you can identify their differences. **Finally**, you’ll identify the command you need to perform a task.

It's time to get ready to explore some of the Linux help resources!

## Task 1. Learn more about commands
In this task, you need to explore a few commands you can use in the shell to learn more about the functionality of other commands.

**First**, imagine you can’t quite remember what the `cat` command does and want a quick reminder.

1. Run the whatis command to get a short description of `cat`.

**Next**, imagine that you want more details about `cat` and all of its options.

2. Use the `man` command to get more details about `cat`.

The man command returns a general description of `cat` and information about each of its options:

```bash
CAT(1)                                                         User Commands                                                        CAT(1)

NAME
       cat - concatenate files and print on the standard output

SYNOPSIS
       cat [OPTION]... [FILE]...

DESCRIPTION
       Concatenate FILE(s) to standard output.

       With no FILE, or when FILE is -, read standard input.

       -A, --show-all
              equivalent to -vET

       -b, --number-nonblank
              number nonempty output lines, overrides -n

       -e     equivalent to -vE

--More--
```
When the first page of information returned by man is displayed, the output pauses.

> ***Note:** You can output more information one line at a time by pressing the **ENTER** key or output the next page of the manual by pressing the space bar.*

3. Press **Q** to exit this manual page.

**Now**, imagine you’ve remembered there’s a command that prints just the first part of a file, but you can’t remember the exact command. The `apropos` command is useful in these instances. You can use keywords with `apropos` to find a command.

4. Use `apropos` to find a command that returns the first part of a file:

```bash
apropos -a first part file
```

> ***Note:** There is no right and wrong when using `apropos` in terms of keywords. Think of it as a very focused search. It will only return commands that correspond to keywords you supply. Keep trying if the first returned command does not provide what you need. Also, keep in mind that using the `-a` option will limit results to only those commands that match all keywords supplied.*

## Task 2. Explore the useradd command
In this task, imagine that you want to set the expiration date for a temporary user account. You know that you need to use the `useradd` command for this, but you’re not quite sure how to complete the task. You realize it might involve adding an option to the command.

1. Use the most appropriate Linux command to get help on the `useradd` command and learn more about all of its options.

> ***Note:** You can output more information one line at a time by pressing the **ENTER** key or output the next page of the manual by pressing the space bar.*

2. Press **Q** to exit this manual page.

## Task 3. Explore the rm and rmdir commands
In this task, you need to determine the difference between the `rm` and `rmdir` commands.

Imagine that you’ve used these commands before, but you can’t remember how they’re different.

- Use the most appropriate Linux command to quickly remind yourself what each command does.

> ***Note:** This task will require entering two commands, one with `rm` and one with `rmdir` .*

## Task 4. Determine which command to use
In this task, imagine that you need to create a new group but you can’t remember what command to use. You need to identify a command that will do this by searching for it through keywords. In this case, use the keywords `create new group`.

- Use the most appropriate Linux command with these keywords to identify what command to use.

## Conclusion
Great work!

You now have practical experience in using basic Linux Bash shell commands to

- get a short description of a command,
- display the man pages for a command, and
- find commands based on keywords about their function.

This ability will be valuable as you navigate the Linux command line.