## 1. Create a new repository

### 1.1. Make a new repository in GitHub
I made a new repository named as 'git_practice'. Then, I got the repository on 'https://github.com/phoenix2718/git_practice'.  

### 1.2. Clone the repository on your local directory
```
git clone https://github.com/phoenix2718/git_practice
```

### 1.3. Make a remote connection between the repository in my GitHub and the local directory
First, change the working directory to the local directory.
```
cd <folder name>
cd git_practice
```
We should make a connection between the repositry in GitHub and the local directory.
```
git remote add <connection name> <repository url in github>
git remote add git_practice https://github.com/phoenix2718/git_practice
```
We can check what connections exist by typing as follows.
```
git remote -v
```

### 1.4. Push new files into the new repository.
iAfter you added some files in the local directory, you would like to add the new files into the repository in the GitHub server. 
First, add all files to the list to commit. '.' means all files in the present working directory.
```
git add <file>
git add .
```
Second, make a commit of all files with a message.
```
git commit -a -m <string message>
git commit -a -m "String message"
```
Third, push the commit to the remote directory in GitHub.
```
git push <connection name> <user name>
git push git_practice master
```
Once you enter the command, you should type GitHub ID and password to push. Then, you can find that the new files are added in 'https://github.com/phoenix2718/git_practice'.


