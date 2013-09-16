# Using Github for Class

## What's Git?
Git is a version control software. It tracks changes that you make to text files over time, and allows you to easily access previous versions of files. It also makes collaboration much smoother when multiple people are working on the same set of files by identifying and helping to resolve conflicts that arise when the same file has different changes.

### Git Project Structure
A git project (or *repository*) lives in a folder. There's no specific structure to the contents of that folder: it can contain whatever files and subfolders you want it to. Git runs in the background and watches your files for changes.

That said, you still have to tell git what you want it to remember. This is done through *commits*. Before a set of changes can be committed, the changes must be *staged*, telling git which changes you want to commit. A commit must be accompanied by a *commit message* describing what changes have been made since the last commit.

This sounds complicated and not highly advantageous at first, but it ends up being a pretty quick and easy process, and it can save you huge amounts of headache down the road. If, at some point, you realize you have made a huge mistake and ruined everything, git makes it easy to *roll back* your changes and return to a previous project state.

## What's Github?
Github is an online resource for hosting git repositories in a place where anyone from a team can access them. Github adds two really important actions, called *pushing* and *pulling*. *Pulling* a project brings the changes from a Github repository into the repository you have on your computer. *Pushing* a project takes any changes you have made and applies them to the *remote* repository on Github.

## What You Need To Know
Git is an incredibly powerful and complex tool that you should learn about on your own if you're interested, but for the purposes of this class we will only be using a few commands.

### Diving Into The Command Line
The command line (or Terminal) can be quite scary at first. It's not bad. You probably won't break the computer. The command line is actually very simple and easy to use. The navigation style is similar to Finder in that you navigate between hierarchies of folders (directories), only the level of visual feedback is greatly reduced. Here are a few important commands you'll need to navigate the command line:

`ls -la`: This will give you a list of the files and folders that are available in the current directory.

`cd DIRECTORY_NAME`: cd stands for Change Directory, and it will allow you to move into any of the folders shown when you do `ls -la`. Replace `DIRECTORY_NAME	` with the name of the directory you want to move into. 

If you want to move back into the root directory (represented by Macintosh HD in Finder), run `cd ~`.

To back up one directory, run `cd ..`.

`pwd`: This will help you out a whole lot if you get lost. Running `pwd` gives you the path to the current directory.

`mkdir DIRECTORY_NAME`: This will create a new directory inside of the current directory. Replace `DIRECTORY_NAME` with whatever you want the directory to be called.

### Introducing Git In The Command Line
In the command line, the first word of any command refers to the  program that executes the command. Any subsequent words are instructions and options for what you need that program to do. For example, `cd` is the UNIX program for changing directories. When you say `cd DIRECTORY_NAME`, you're telling the program `cd` to execute, and you're telling it to use `DIRECTORY_NAME` as the input that it requires. Git is like any other UNIX program that you run from the command line. All git commands will begin with `git` followed by more specific instructions.

`git pull`: As a rule of thumb, whenever you sit down to work, run this first. It will make sure that your repository is up to date with the one on Github.

`git add .`: This is the easiest way to stage all of your changes and start tracking any new files. You will need to run this before you commit in order to tell git that you want it to take note of the changes you have made.

`git commit -m "YOUR COMMIT MESSAGE HERE"`: This will commit your changes locally. `-m` is telling git that whatever comes next in quotes is the commit message.

`git push`: This will push your changes to the remote repository. It's usually a good idea to run `git pull` before `git push`; if there are changes to the remote repository that have been made since your last pull, the push will fail and you will get an error message.

`git status`: This will give you a rundown of what changes are staged for commit, what changes haven't been staged yet, and what files haven't been tracked yet. It's good if you aren't sure whether you have changed anything since your last commit.






