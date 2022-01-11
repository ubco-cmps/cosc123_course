# Lab 1

This lab has three tasks, they are all independent and you can do them in any order:

- Task 1: Install the Processing programming development environment (PDE)
- Task 2: Go through the install instructions for your operating system (macOS, Windows, Linux)
- Task 3: Complete the GitHub Tutorial.

## Task 1: Install Processing (12 marks)

To install the Processing Development Environment (PDE), you should follow these steps:

1. [Visit the download page](https://processing.org/download/).
1. Download the installer for the latest version (v3.5.4) your operating system (Windows, macOS, or Linux)
1. See the installation instructions for your operating system ([adapted from here](https://processing.org/tutorials/gettingstarted/)):

    - On Windows, you'll have a .zip file. Double-click it, and drag the folder inside to a location on your hard disk. I suggest a location where your other programs are stored. Once it's moved out of the unzipped folder, you can double-click processing.exe to start.

    - On macOS, the installer is also a .zip file. Double-click it and drag the Processing icon to the Applications folder. Then double-click the Processing icon to start.

    - The Linux version is a .tar.gz file. Download the file to your home directory, then open a Terminal window, and type: `tar xvfz processing-3.5.4-linux64.tgz`. This will create a folder. Then change to that directory: `cd processing-3.5.4` and then run it by typing `./processing`.

## Task 2: Prepare your System (40 marks)

There are several things you need to install on your machines for this course.

- On macOS, follow the instructions [here](./macOS.md).

- On Windows, follow the instructions [here](./windows.md).

- On Ubuntu, follow the instructions [here](./ubuntu.md).

Once you have gone through the installation instructions, please take a screenshot with the following requirements:

- One terminal window with the output of `git config --list --global`
- Another terminal window with the output of `code --version` and `git --version` sequentially printed
- Processing open with the following code run: `ellipse(15,30,25,50);`
  - If you have not yet installed Processing, you should now go back and complete Task 1
- VS Code open
- Date/time should be visible somewhere in the screenshot

Here is an example of what you should be aiming for:

<img src="https://github.com/firasm/bits/blob/master/install_proof.png?raw=true" width=100%>

### Acknowledgements

These installation instructions were heavily adapted from the ones found [here](https://ubc-mds.github.io/resources_pages/installation_instructions/).

## Task 3: GitHub Tutorial (48 marks)

I will be honest: Git and GitHub is a difficult thing to teach so after many years of searching, I have found the [**PERFECT** tutorial](http://learngitbranching.js.org).
This tutorial wil help you get more familiar with git commands, particularly branching, and merging - things you will start encountering when you start collaboratively working in your repos.

At minimum, you are responsible for completing the following modules:

- "Main: Introduction Sequence"
  - Exercise 1
  - Exercise 2
  - Exercise 3
  - Exercise 4
  
- "Ramping up"
  - Exercise 1
  - Exercise 2
  - Exercise 3
  - Exercise 4

- "Remote: Push & Pull -- Git Remotes"
  - Exercise 1
  - Exercise 2
  - Exercise 3
  - Exercise 4
  - Exercise 5
  - Exercise 6
  - Exercise 7
  - Exercise 8

- "To Origin And Beyond -- Advanced Git Remotes!"
  - Exercise 1
  - Exercise 2
  - Exercise 3
  - Exercise 4
  - Exercise 5
  - Exercise 6
  - Exercise 7
  - Exercise 8

You will get 2 points for each activity, for a total of 48 points.

Once you are done, you should include a screenshot of both the exercises in "Main" and "Remotes", and also include a text file where you write your github username and the current date/time.

Here is an example of the screenshot we are expecting (if you want full marks you will have completed all 24 exercises).

<img src="https://github.com/firasm/bits/blob/master/github_tutorial.png?raw=true" width=100%>