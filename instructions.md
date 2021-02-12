# A quick Git guide to make your first steps

Today we'll learn how to correct a typo in one of our files and add our suggestions for changes.

We'll do it with the help of the terminal: in a nutshell, it's a way to accomplish and automate tasks on your computer. Today it'll help us work with Git right from your desktop. Type "terminal" in a search box and open the application.


## Correcting a typo
We are going to practice using the GitHub repository called "PracticeRange". Inside there is a text file called "text1" we need to correct. We are going to clone this repository to our laptop, correct a typo and upload the repository back to GitHub.

1. Open the repository "[PracticeRange](https://github.com/ArcticDreamer/PracticeRange)", click the "Code" button, and copy the HTTPS address.

2. Open the terminal and type the command + the HTTPS address you just copied:

`git clone https://github.com/ArcticDreamer/PracticeRange.git`

The repository is now saved on your laptop.

3. Open the folder "PracticeRange" on your laptop, find the "text1" file that needs to be corrected, and fix the typo. The file is ready to be updated to the main repository.

4. Switch back to the terminal. Let's indicate that we want to work with the files inside the "PracticeRange" folder.

`cd PracticeRange`

5. Mark the file that you want to upload — that's how the terminal will understand what is ready to be moved to the repository.

`git add text1`

6. Let's commit this file, or, in other words, upload the fixed file to the repository. You must leave a comment explaining what kind of change you commit.

`git commit -m «correct a typo»`

7. Now that you've made the changes on your laptop, let's upload the updated repository to GitHub.

`git push`

Now you can update the GitHub page and make sure the typo's fixed.


## Making suggestions
If you see a sentence in a text file "text2" and realize you know a better way to express the idea, yet you are not so sure it is worth changing the whole file, there is a way you can leave your suggestions.

You can make a separate branch of the "PracticeRange" repository on your laptop, change a part of the text you don't like and upload the new branch to GitHub. The original version of the repository will still be on GitHub, and your colleagues will be able to compare your version with the original one.

1. Let's update the files that we already have on our laptop to be sure we have the latest version of our repository.

`git pull`

2. Indicate that we are going to work with the folder called "PracticeRange".

`cd PracticeRange`

3. Create a new branch called "Practice2". It will be identical with the original repository, and you'll be able to experiment with it's content without any fear of messing things up.

`git branch Practice2`

4. Switch to the new branch.

`git checkout Practice2`

5. Open the "text2" file, correct the sentence you want and switch back to the terminal.

6. Mark the file that you've corrected and want to commit.

`git add text2`

7. And commit it to the repository. You must leave a comment as well explaining what kind of change you commit.

`git commit -m «correct a typo»`

8. You've made the changes on your laptop. Now let's upload the new branch to GitHub.

`git push origin Practice2`

Refresh the GitHub page and make sure the new branch has been created. You'll see a GitHub notification suggesting you make a pull request — follow the hints to create a pull request with the comments to your colleagues on why your changes are important.


> A couple of git commands that might be handy:
> - If you want to make sure the command you just ran worked as planned, type `git status` to check.
> - If you are lost in branches, `git branch` will show you where you are.
