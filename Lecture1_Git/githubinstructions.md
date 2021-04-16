# These instructions assumed that you have some knowledge of bash shell
## Start with your bash shell
**Create a directory**
```
mkdir git_ace
```
**Get in the directory to start building your project**

```
cd git_ace
```

**Initiates a local git repository**

```
git init
git status
```

**Create your first file**
```
touch testfile.txt
```
**Check if this file is there in the directory you are in**

```
ls -l
```
**Check if git know about it**

```
git status
```
you might have noticed that git does not know about it

**adding file to git**
```
git add testfile.txt
git status
```
**Committing file**
```
git commit testfile.txt -m "trying to commit my first file"
```
**Here are the list of above steps you will see on your terminal**
![Alt text](imgs1/local_git.png)

## Go online and create a new repository with the same name as you create locally on your machine (name: git_ace)
**Below are the steps to follow**

![Alt text](imgs1/new_repository.png)
![Alt text](imgs1/create_repository.png)
![Alt text](imgs1/setup_repository.png) 

**The final step is to push your changes or files from local repository to your new remote repository
```
git remote add origin https://github.com/skumarudel/git_ace.git
git remote -v
git push -u origin master
```
**Modify the file and push the changes to remote repository**

```
echo "First line of code" >> testfile.txt
git status
git add testfile.txt
git commit testfile.txt -m "Modify the file"
git push
```
Go online to your repository and see if the changes you made appear or not?