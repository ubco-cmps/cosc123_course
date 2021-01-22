# COSC 123 Lab 2 - Command Line Practice

## Instructions

For this lab, you will follow the instructions below.
This week, you will be practicing the command-line through a game. 

I have a recorded video for this lab from another course, and I encourage you to watch it as an introduction to Lab 2. 

```{dropdown} Introduction to Lab 2
    :container: + shadow
    :title: bg-primary text-white font-weight-bold
    :open:

<div class="container youtube">
<iframe class="responsive-iframe" src="https://www.youtube-nocookie.com/embed/kr4ndlFYYes" frameborder="0" allow="accelerometer; autoplay="0"; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
```

## Objectives

- Practice with command-line interfaces
- Create and navigate directories
- Create, modify, rename and delete files
- Understand Git and Git fundamentals

## Marking and Evaluation (10 marks)

**Step 1: Accept the lab assignment**
You can find the link to accept the lab at the usual place on "Canvas", under "Course Content", after clicking "Lab Stuff".

**Step 2: Clone the repository on your local computer and navigate to that directory**

As with Lab 1, you will need to clone the GitHub repository somewhere locally.
The steps to do this are:

1. `cd /path/to/where/you/want/labs`
2. `git clone https://github.com/cosc123-2020-winter2/lab2-yourUserName`

You will get these marks if you follow these, and the other instructions below.
Any deviations from the instructions below, and you'll lose marks from this section.

## BashCrawl (70 marks)

BashCrawl is a text-based game/tutorial to help you get comfortable with the Terminal.

### Setting up for the game

1. Open a Terminal window.
2. Change the directory to where this file is: `cd /path/to/this/folder`.
3. Type `ls` into the Terminal; you will see two things: `README.md` and the `entrance` directory.
4. Once you go into the `entrance` directory (`cd entrance`), the command line based game will begin!

**Tip: When I say "go into the <BLANK>" room, I mean change directories using `cd <BLANK>`. In this game, a "room" is a "directory".**

### Starting the game

5. Now that you have entered the dungeon `entrance`, you should type `ls` in the terminal to look around and see what's there.
6. You will see there are two "things" in this room,  there is a `scroll`, and another room called `cellar`.
7. Let's read the scroll using `cat scroll`.

**Tip: When I say "read the scroll", I mean output the contents of the scroll file into the Terminal using `cat scroll`.**

8. Great! The scroll told us that we can look and see what's in the room using `ls` and move in and out of rooms using `cd <directory>`. Let's go into the cellar: `cd cellar`.

9. Once we're in the `cellar`, let's have a look around: `ls`. You should see an `armoury`, a `scroll`, and some `treasure`.

10. Let's read the scroll: `cat scroll`. It should tell you about `ls -F`. Here is some more information about `ls -F`:

> Display a slash (`/') immediately after each pathname that is a directory, an asterisk ('*') after each that is executable, an AT sign ('@') after each symbolic link. 

11. That sounds useful, let's do an `ls -F` in the cellar to see what each of the things are. You'll notice that the armoury is another room, the scroll is just a file, and the treasure has a "*" at the end, so it's an executable. Cool! We don't know what to do with the executable yet, but let's try `cat treasure` to see what happens.

12. Mm. Didn't work - okay let's move on and come back to this room later. Let's go into the `armoury` now: `cd armoury` and then `ls -F`.

13. We see another scroll (and a potion, a treasure, and another room)! Let's read the scroll: `cat scroll`.

14. Oooh, we have now learned how to collect `treasure`! Let's do that in the armoury and follow the instructions to keep our treasure (using environment variables).

**Tip: When I say "pick up the <BLANK>", I mean run the executable file using `./ <BLANK>`.**

15. It tells us to go back and get the treasure from the cellar! Let's go and do that now with `cd ..`, pick up the treasure from the cellar, and then come back to the armoury.

16. The potion is also something we can "pick up", so let's go ahead and do that. It asks us if you want to drink it: type 'Y' for yes, and anything else for no (like 'n'). Choose an option and see what happens (follow on-screen instructions!)

17. Alright check if there's anything else to do this in room, if not, head to the `chamber` next. Start with `ls -F` and hopefully by now, you know the drill!

18. Have fun! More dungeon rooms will open up as you complete certain tasks, kill certain monsters, and read specific scrolls and tomes. Have fun with it, this is your opportunity to practice your Terminal skills - it sure beats the way I learned Terminal commands (blindly typing in commands in a black box until I got it to do what I wanted!). There is no need to hit **every** room in the dungeon, but if you make a good effort to explore the dungeon, you'll likely get most of the marks for this lab. In your scheduled lab this week, the TAs will discuss a bit more on how this will be graded.

**Tip: You can ignore a few of the more "advanced" entries of the Tome, including anything related to `tmux` or `gzip`.**

## Submitting Lab 2 (20 marks)

When you're done exploring the dungeon there are several things you need to do to complete the lab and get the marks for this section.

### 1. Commit everything to your repository and push to the cloud:

```
git add . (or git add -A)
git commit -m "Finished playing with the dungeon"
git push
```

### 2. Generate a full dungeon hierarchy using "tree"

**Windows** instructions:

- GitBash *should* have the `tree.com` program already installed on your computer. If it is not (i.e. if you get a command not found when you tried the commands below), then I'd suggest creating a new post on Ed Discussion or going to a TA or instructor office hour. 

- Open a new GitBash window, simply `cd` (change directory) into your lab2 directory, and run these commands:

```
tree.com \\a \\f
tree.com \\a \\f > mydungeonmap.md
```

**macOS** instructions:

- Chances are `tree` is already installed on your Mac. To check if it is, type `which tree` in a Terminal window, and it will report the location of this program (you don't need the location, but it will look something like: `/usr/local/bin/tree`)

- Once you've confirmed `tree` is installed on your machine, simply `cd` (change directory) into your lab2 directory, and run this command:

```
tree
tree > mydungeonmap.md
```

The first command will generate a hierarchy of all files and folders in your lab2 directory. 
The second command will put the results of `tree` into `mydungeonmap.md` to create your explored dungeon map!

**Linux** instructions:

- `tree` should already be installed on Linux, to check if it is, type `which tree` in a Terminal window, and it will report the location of this program (you don't need the actual location, just that it's installed).

- Once you've confirmed `tree` is installed on your machine, simply `cd` (change directory) into your lab2 directory, and run this command:

```
tree
tree > mydungeonmap.md
```

The first command will generate a hierarchy of all files and folders in your lab2 directory. 
The second command will put the results of `tree` into `mydungeonmap.md` to create your explored dungeon map!

### What to do if `tree` isn't installed on your machine? 

Generally speaking, if `tree` is not installed, you will be better off coming to a lab or office hour to get some help. You can try doing it yourself below, but the install instructions will be different based on your operating system.
If you're struggling, come talk to us and don't leave things till the last minute!

#### **Windows**

If you believe `tree.com` is not installed on your machine, please create a post on Ed Discussion or reach out to a TA during office hours or during a lab

#### **macOS**

- In case `tree` is NOT installed, you can do so by first trying: `brew install tree` but if you do not have Brew installed, you will need to install that first using this command: 

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Alternatively, if you have miniconda or anaconda installed, you can try: `conda install -c conda-forge tree`

#### **Ubuntu**

sudo apt-get install tree

In case `tree` is NOT installed on Ubuntu, you can do so by trying: `sudo apt-get install tree` or `snap install tree`, or `yum install tree` depending on your favourite backage manager.

### 3. Commit the dungeon map to your repository 

Run the following commands in your Terminal:

```
git add .
git commit -m "Added my dungeon map"
git push
```

### 4. Save the last 100 commands from your Terminal

We want to see some serious effort with the dungeon map, so we are asking for the last 100 commands you entered into the Terminal.
The `history` command will report commands that you ran.

```
history 100 > dungeonHistory.md
```
Please open this file and do a quick check to make sure there is no sensitive information in this file (like passwords or private messages).
If there is, you can simply edit file or remove that command.

**Note: Just because we're asking for the last 100 commands doesn't mean that we expect you to have 100 commands, you may have less and you may have more. That's fine.**

### 5. Commit the dungeon history to your repository 

Run the following commands in your Terminal:

```
git add .
git commit -m "Added my dungeon map"
git push
```

### 6. Submit the link to your GitHub.com repo to Canvas

You're done! 

## Attribution

The `bashcrawl` game was adapted from `@slackermedia` on GitLab.
FULL Credit for the game goes to [Seth Kenlon](http://slackermedia.info/about/).
The link to the game source code is [here](https://gitlab.com/slackermedia/bashcrawl).