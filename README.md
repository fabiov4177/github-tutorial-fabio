# GitHub Tutorial

_by Fabio Velasquez_

---
## Git vs. GitHub
**Git:**

- Git is a _version control system_, what this means is that it keeps "snapshots" of code
- Git is an amazing way to manage your code, every developer uses it
- HTML, CSS, JS, Ruby, SQL, Python, Java, Swift, Arduino all stored on Git 
- Git does not require the use of GitHub

**Github:**

- Github is the _cloud_, or place where the code is stored
- You can see the changes you have made and keep track of them
- It is easy to work with other people on GitHub, and you can collabrate on files
- Github requires the use of Git 


---
## Initial Setup
**Signing up for GitHub**:

- Go to [https://github.com/](https://github.com/) and click on Sign Up
- Select and enter your own Username, Email Address and Password
- Select your plan
- Finish the rest of the Setup

**Setting up an SSH Key:**

- Grab the SSH Key from your IDE
- On the top right of your GitHub, click on your profile icon and go to settings
- Where it says "Personal Settings" on the left sidebar, click on SSH Keys
- Then click on "Add SSH Key" and type in the SSH Key you got from your IDE, and the title of it is your choice, then click "Add Key"
- Then on your IDE, type in `ssh -T git@github.com` and type _"yes"_ to confirm it

**Configuring:**

- Type in `git config --global user.name "First Last"`
- Also type in `git config --global user.email "Email Address"`



---
## Repository Setup
For example purposes were going to use the name practice-repo, and README.md but note you don't have to call it this, you can name it whatever you want, this is just an exmaple!

1. In your IDE type `mkdir practice-repo`
2. Go into it by typing in `cd practice-repo`
3. Type `git init` to initalize the repo
4. Add a new file so type in `touch README.md` to create a starter file
5. Save your file or if you're using Auto Save on your IDE, skip this step
6. Add this file to the stage by typing `git add README.MD`
7. Type in `git commit -m "your message here"`
8. On your GitHub account, on the top right click on the "+" button and click "New repository"
9. Fillout the repository information and makre sure that **both repos on your IDE and on Github both have the same name**
10. Then click "Create repository"
11. Now type in your IDE
12. ```
    git remote add origin git@github.com:(your username)/practice-repo
    git push -u origin master ```
    
9. Then finally just type in `git push` and all your changes to your repo will be "pushed" to your remote


---
## Workflow & Commands
The workflow is save, add, commit, push

`git add` adds your file to the Git stage, which means that your file is ready to be committed. You type in `git add "your file name"`

`git commit` is when Git takes the snapchat of what is on the stage. Also you are aloud to add a message to your commit to help you describe what you changed to your file in this commit, the way you type it in to your IDE is `git commit -m "whatever your commit message is"`

`git push` is the last part of the Workflow, this is where you are "pushing" your changes to the cloud, which is GitHub. The way you type it in is just `git push` and you will see all your changes being pushed up to Github.

##Note:

Throughout this work flow it is a good idea to use the command `git status` in between each step.

`git status` is a command that helps you keep track of whats going on. What I mean by this is it helps you know whats being added to the stage, or what is being committed, or what file hasn't been changed. It is an important part of the workflow as it helps you know whats going on and keeps you up to date and on top of things.


___
## Error Handling



___
## Collaboration