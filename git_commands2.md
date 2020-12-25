

# git init

**git init** stands for git initialize. Its used to turn a folder into a git repository(oppbevaringsted).
```
git init 
```
After you turned your folder into a git repository, you can se that there is a hidden directory called **.git** in that directory. You can se that by typing

```
ls -a
```
You can also do

```
ls .git

```
To se what is inside **.git** directory. This is the internal directory where git stores all its internal data, namely **objects** and **referenses**

# git help <command>

Git help takes a sub command as an argument and gives you information about it. 
for example 

```
git help init
```

# git status

This tells you whats going on in the repository

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

`
