## Research Questions 

Now that you are all set up, it's time to learn a little more about the tools of the trade. Edit this file and answer the following questions. You are going to need to start familiarizing yourself with the [GitHub docs](https://docs.github.com/en). Docs (short for documentation) are the instructions on how to use a languge or program. A large part of your job as a developer will be learning how to read and work with documentation. Please reference the GitHub docs when answering the questions below. If you cannot find what you are looking for in the docs, you can always start to practice your Google skills!

1. What is Git?
Git is a tool that web devs use to manage source code. 
Developers use it for asynchronous development; it's a control system.

2. What is the difference between Git and GitHub?
GitHub is a cloud-based hosting service that allows you to host your Git repositories! There are many of these services, but I do prefer GitHub.

3. Why do we create a branch? 
We create a branch to avoid crowding the main branch with conflicting commits from other developers. It allows you to make mistakes without destroying all of your code ;)

4. What is the purpose of a Pull Request?
Pull Reqs are used in large-scale contributions. A senior developer will look at your pull request and examine the differences between your branch and the main branch. 

5. What is the command you can use to switch between branches? For example you are working on FIRSTNAME-LASTNAME branch and you want to switch back to main.
First, type `git branch` to determine what branches are available.
Next, type `git checkout <branch>`. (example, `git checkout main`, or `git checkout arbor-matos`)

6. Explain the difference between `git fetch`, `git merge` and `git pull`. What does each command do?
`git fetch` downloads objects and other assets from a remote repository.

`git merge` takes independent lines of development created by multiple users' branches and puts them into one (1) branch.

`git pull` is kind of like a one-stop-shop for fetching and merging all the changes from a remote repository.


7. What is a merge conflict?
Merge conflicts arise when changes are made to the same line of a file by multiple different people (more than one). It can also happen when one person tries to edit a file and another person simply deletes the file.

8. How do you resolve a merge conflict?
To resolve a merge conflict, navigate into the local repo that has the conflict via the terminal.
Type `git status`; it will tell you what branch you've got conflicts on, and in what files.
On Mac, you can type `code .` to open VSCode (or another text editor) and search for the conflict marker `<<<<<<< HEAD`, followed by one line of code, the branch partition `=======`, another line of code, and the the end of the conflict marker `>>>>>>> BRANCH-NAME`. It will all look like this put together: 


good morning,
`<<<<<<< HEAD`
sleepy head~!
`=======`
starshine, the earth says hello!
`>>>>>>> arbor-matos`

(You'll see it without the backticks, but without backticks it actually registers as a conflict and will not be pushable lmao)


Determine which version you want to keep, delete the conflict tags, stage your changes, and commit. 
The end result will look super natural and such:



Good morning, starshine, the earth says hello!