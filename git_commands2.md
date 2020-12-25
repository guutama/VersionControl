

# git init

**git init** stands for git initialize. Its used to turn a folder into a git repository(oppbevaringsted).
```
git init 
```
After you turned your folder into a git repository, you can se that there is a hidden directory called **.git** in that directory. You can se that by typing

```
ls -a
```
To se what is inside **.git** directory. This is the internal directory where git stores all its internal data, namely **objects** and **referenses**
```
ls .git

```


# git help <command>

Git help takes a sub command as an argument and gives you information about it. 
for example 

```
git help init
```

# git status

This tells you whats going on in the repository

```
git status

```

# Staging area
Is were you put everything you want to include in the next snapshot(next version)  you take. You add your file or folder to the staging area by:

# git add <name_of_file/folder>

To put a file in staging are
```
git add hello.txt

```

To put a folder with all its content in staging area
```
git add MyFolder

```

To add everything from your top-level directory to staging area

```
git add :/
```


# git commit

Takes all the files and folders in the staging area and create a new snapshot.

The following command takes you to your default text editor, so you can write a message that tells about the changes made in this version(snapshot). 
```
git commit 

```
You can also white the message in command line

by

```
git commit -m "Your message"
```

Its really important to write high quality commit messages, because letter when you looking back in your projects version history,you know why you made certain changes


You can commit without out staging area. The following command will commit all files that has already been tracted by git and been modified

```
git commit -a

```


# git log

The git log command helps you visualize the history, the commit graph. 
```
git log

```

# git cat-file -p <hash-number_of_commit>

This command prints the content of the commit. You dont need to spesify the whole 40 char of commid id. It usually holds with first 5 or 6
```
git cat-file -p 43f455

```


By default the git log command shows you flattened version of history, it will linearize and show you in order.
But git log can also take an argument that shows history as graph

```
git log --all --graph --decorate

```
The more recent commit shown at the top.



# References 
Refereences are way of naming things in the repossitory in humen redable names. 


# main

Main is referense that is created my default when you initialize a directory with git repasitory. This name was changed from **master** to **main** in 2020. By convention this referes to the main development in your code. so main will represent the most upto date version of your project history. 

# HEAD
HEAD is spesial referense in git. It referes to where you are looking at at the moment. 


# git checkout

This command lets you do bunch of things. One of the thigs you can do is to move around your version history.

## git checkout <commit hash/id>
Lets you change the state of your working to that of the given ID. you can see that by **git log** that HEAD is now pointing to another place. 
```
git checkout 4f3456

```

You can also give the name of the branch rather than ID

```
git checkout main

```





## How does git related to github

Github is a repository host for git. You can create a repository on github and store a git repository on github, and use that to colaborate with other people. Git as acommandline tool is independant from gihub. You dont have to use github to use git, and you dont have to use github to colarate with other poeople. 
 
