# Activity: Install software in a Linux distribution

## Introduction
In this lab, you’ll learn how to install and uninstall applications in Linux. You’ll use Linux commands in the Bash shell to complete this lab. You’ll also use the Advanced Package Tool (APT) package manager to install and uninstall the Suricata and tcpdump applications.  

> **Disclaimer:** For optimal performance and compatibility, it is recommended to use either **Google Chrome** or **Mozilla Firefox** browsers while accessing the labs.

## What you’ll do

You have multiple tasks in this lab:

- Confirm APT is installed in Bash

- Install Suricata with APT

- Uninstall Suricata with APT

- Install tcpdump with APT

- Reinstall Suricata with APT

## Lab instructions

### Start the lab
Before you start, you can review the 
[Resources for completing Linux labs](/Linux%20and%20SQL/Module%202/resources-for-completing-linux-labs.md). Then from this page, click **Launch App**. A Qwiklabs page will open and from that page, click **Start Lab** to begin the activity!

*You may attempt this lab a maximum of 5 times, and you will have 60 minutes to complete this lab during each attempt.*

### End the lab
From within the lab, click **End Lab** to end your lab. 

Additionally, sometimes you need to refresh your Coursera page in order for your progress to be registered. If you refresh this page after you complete your lab, the green check mark should appear.

#### Best practices for completing labs:

- Make sure your browser is up to date with the latest version.

- Make sure your internet connection is stable.

- After you complete the lab, leave the lab window open for at least 10 minutes in order to allow the system to record your progress.

- If you run into issues connecting to the lab, try logging into Coursera in an Incognito mode and completing the lab there.

- Review [Lab tips and troubleshooting steps](/Linux%20and%20SQL/Module%202/lab-tips-and-troubleshooting-steps.md)for more information.

---
This course uses a third-party app, Activity: Install software in a Linux distribution, to enhance your learning experience. The app will reference basic information like your name, email, and Coursera ID.
---
## Activity overview
In this lab activity, you’ll use the Advanced Package Tool (APT) and sudo to install and uninstall applications in a Linux Bash shell.

While installing Linux applications can be a complex task, the APT package manager manages most of this complexity for you and allows you to quickly and reliably manage the applications in a Linux environment.

You'll use Suricata and tcpdump as an example. These are network security applications that can be used to capture and analyze network traffic.

The virtual machine you access in this lab has a Debian-based distribution of Linux running, and that works with the APT package manager. Using a virtual machine prevents damage to a system in the event its tools are used improperly. It also gives you the ability to revert to a previous state.

As a security analyst, it's likely you'll need to know how to install and manage applications on a Linux operating system. In this lab activity, you’ll learn how to do exactly that!

## Scenario
Your role as a security analyst requires that you have the Suricata and tcpdump network security applications installed on your system.

In this scenario, you have to install, uninstall, and reinstall these applications on your Linux Bash shell. You also need to confirm that you’ve installed them correctly.

Here’s how you'll do this: **First**, you’ll confirm that APT is installed on your Linux Bash shell. **Next**, you’ll use APT to install the Suricata application and confirm that it is installed. **Then**, you’ll uninstall the Suricata application and confirm this as well. Next, you’ll install the tcpdump application and list the applications currently installed. **Finally**, you’ll reinstall the Suricata application and confirm that both applications are installed.

OK, it's time to learn how to install some applications!

> ***Note:** The lab starts with your user account, called `analyst`, already logged in to the Bash shell. This means you can start with the tasks as soon as you click the **Start Lab** button.*
> **Disclaimer:** For optimal performance and compatibility, it is recommended to use either **Google Chrome** or **Mozilla Firefox** browsers while accessing the labs.

## Start your lab
Before you begin, you can review the instructions for using the Qwiklabs platform under the **Resources** tab in Coursera.

If you haven't already done so, click **Start Lab**. This brings up the terminal so that you can begin completing the tasks!

When you have completed all the tasks, refer to the **End your Lab** section that follows the tasks for information on how to end your lab.
---
## Task 1. Ensure that APT is installed
First, you’ll check that the APT application is installed so that you can use it to manage applications. The simplest way to do this is to run the apt command in the Bash shell and check the response.

The Bash shell is the command-line interpreter currently open on the left side of the screen. You’ll use the Bash shell by typing commands after the prompt. The prompt is represented by a dollar sign ($) followed by the input cursor.

- Confirm that the APT package manager is installed in your Linux environment. To do this, type `apt` after the command-line prompt and press **ENTER**.

When installed, `apt` displays basic usage information when you run it. This includes the version information and a description of the tool:

```bash
apt 1.8.2.3 (amd64)
Usage: apt [options] command

apt is a commandline package manager and provides commands for
searching and managing as well as querying information about packages.
It provides the same functionality as the specialized APT tools,
like apt-get and apt-cache, but enables options more suitable for
interactive use by default.
...
```
APT is already installed by default in the Linux Bash shell in this lab because this is a Debian-based system. APT is also the recommended package manager for Debian. If you’re using another distribution, a different package manager, such as YUM, may be available instead.

## Task 2. Install and uninstall the Suricata application
In this task, you must install Suricata, a network analysis tool used for intrusion detection, and verify that it installed correctly. Then, you’ll uninstall the application.

1. Use the APT package manager to install the Suricata application.

Type `sudo apt install suricata` after the command-line prompt and press **ENTER**.

> ***Note:** The `apt install` and `apt remove` commands must be prefixed with the `sudo` command as elevated privileges are required to install and uninstall software in Linux.
> 
> The Suricata application can take a few minutes to install.*

When you install an application with APT, the output displays details of all the software to be installed. This may include additional applications that depend on the new software. These additional applications are called the dependencies of the software to be installed.

When prompted to continue, press the **ENTER** key to respond with the default response. (In this case, the default response is **Yes**.)

2. Verify that Suricata is installed by running the newly installed application.

Type `suricata` after the command-line prompt and press **ENTER**.

When Suricata is installed, version and usage information is listed:

```bash
Suricata 4.1.2
USAGE: suricata [OPTIONS] [BPF FILTER]

    -c   : path to configuration file
    -T         : test configuration file (use with -c)
...
```

3. Use the APT package manager to uninstall Suricata.

Type `sudo apt remove suricata` after the command-line prompt and press **ENTER**. Press **ENTER** (**Yes**) when prompted to continue.

When prompted to continue, press the **ENTER** key to respond with the default response. (In this case, the default response is **Yes**.)

4. Verify that Suricata has been uninstalled by running the application command again.
   
Type `suricata` after the command-line prompt and press **ENTER**.

If you have uninstalled Suricata, the output is an error message:

```bash
-bash: /usr/bin/suricata: No such file or directory
```
This message indicates that Suricata can't be found anymore.

## Task 3. Install the tcpdump application
In this task, you must install the tcpdump application. This is a command-line tool that can be used to capture network traffic in a Linux Bash shell.

- Use the APT package manager to install tcpdump.
  
Type `sudo apt install tcpdump` after the command-line prompt and press **ENTER**.

## Task 4. List the installed applications
Next, you need to confirm that you’ve installed the required applications. It's important to be able to validate that the correct applications are installed. Often you may want to check that the correct versions are installed as well.

1. Use the APT package manager to list all installed applications.
   
Type `apt list --installed` after the command-line prompt and press **ENTER**.

This produces a long list of applications because Linux has a lot of software installed by default.

2. Search through the list to find the tcpdump application you installed.

The Suricata application is not listed because you installed and then uninstalled that application:

```bash
...
tcpdump/oldstable,now 4.9.3-1~deb10u2 amd64 [installed]
...
```
> ***Note:** The specific version of tcpdump that you see displayed may be different from what is shown above.*

## Task 5. Reinstall the Suricata application
In this task, you must reinstall the Suricata application and verify that it has installed correctly.

1. Run the command to install the Suricata application.

Type `sudo apt install suricata` after the command-line prompt and press **ENTER**.

When prompted to continue, press the **ENTER** key to respond with the default response. (In this case, the default response is **Yes**.)

2. Use the APT package manager to list the installed applications.

Type `apt list --installed` after the command-line prompt and press **ENTER**.

3. Search through the list to confirm that the Suricata application has been installed.

The output should include the following lines:
```bash
...
suricata/oldstable,now 1:4.1.2-2+deb10u1 amd64 [installed]
...
tcpdump/oldstable,now 4.9.3-1~deb10u2 amd64 [installed]
...
```

## Conclusion
Great work!

You now have practical experience with the APT package manager. You learned to

- install applications,
- uninstall applications, and
- list installed applications.

Being able to manage installed applications in Linux is a key skill for any security analyst.

## End your lab
Before you end the lab, make sure you’re satisfied that you’ve completed all the tasks, and follow these steps:

1. Click End Lab. A pop-up box will appear. Click Submit to confirm that you're done. Ending the lab will remove your access to the Bash shell. You won’t be able to access the work you've completed in it again.
2. Another pop-up box will ask you to rate the lab and provide feedback comments. You can complete this if you choose to.
3. Close the browser tab containing the lab to return to your course.
4. Refresh the browser tab for the course to mark the lab as complete.