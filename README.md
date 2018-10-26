# GitHub Tutorial

_by Leslie Lopez_

---
## Git vs. GitHub  
* #### Git 
  * Git is like a version control that runs in the command line.
  * It keeps snapshots and is usuall where most of the works gets done 
* #### GitHub 
  * GitHub is where most of the code is stored 
  * GitHub is what helps you share others information so that later on you can edit it back in git
* #### Git vs GitHub
   * The difference is that in you git you create the work and edit. Then in GitHub the work is stored and you can see the changes you have made 


---
## Initial Setup
##### Create Account
1. Start by creating an account in [GitHub](www.github.com)
2. Log into your cloud 9
3. Create a workspace 

##### SSH key  
1. Log into your GitHub account
2. Go to top right corner and click on the icon then settings
3. You will see a SSH and GPG key on the left bar  
      * Click on the SSH key  
1. Go to [c9.io](www.c9.io) 
2. Click the gear icon on the top right
3. Choose SSH and copy the whole 2nd link
4. paste the linnk to github
    5.Click on the SSh key
1. Go back to c9 and open workspace
2. type `ssh -T git@github.com `

---
## Repository Setup

* **When creating a folder**  
1.`cd folder`( this makes you go into the folder)  
2.Go into the file and `git init`(this initialize the repo)  

* **Remote Repo in GitHub**  
1.Go to [github.com](www.github.com)  
2.Click + button on top right  
3.Choose _New Repository_  
4.Name the repo the same one you wrote on your c9  
5.Press _Create Repository_  

* **Add, Commit, and Push**  
  1. Clicking command s (This is to save your work)
  2. Git add. (This is to add your work)
  3. Git commit -m "message" (This add a reminder to what you did in the command line)
  4. Git push -u origin master (You type this when pushing to git hub got the first time)
  5. git push (After the first time of pushing use this command for the rest of the pushing to github)


---
## Workflow & Commands
##### General Command Line

| Command | Explanation|
|:-------:|:----------:|
| `ls` | List the files |
| `cd . .`| Goes back a file |
| `mkdir` | Makes a file |
| `rmdir` | Removes a Directory |
| `rm` | Delete a file only if empty |
| `rm rf-` | Delete a file completely |
| `mv` (to rename) | Rename a file created |
| `mv` (to move) | To move a file to another place |
| `c9 file`| Open Preview to different tab|
| `clear`| Have a clear screen |
| Up arrow | Look though previous codes|

##### Git And GitHub

| Command | Explanation|
| :-----: | :--------: |
| `git init` | initialize git |
| `rm -rf .git` | Uninitialize git |
| `git add . ` | will not add deleted or renamed files |
| `git add --all`| Add all previous changes |
| `git commit -m` "message"| To commit a file with a helpful message |
| `git remote -v`| Makes connection to GitHub |
| `git push -u origin master`| Pushed command to GitHub |
| `git status`| Shows changes that need to be made |
| `git log`| Logs changes |

---
## Rolling Back Changes

* **Undoing Add, Commit, and Push**  
  1.`git checkout file` (undoing edits)  
  2.`git reset HEAD file` (Undoing Add)  
  3.`git reset HEAD~1` (Undoing Add from Push)  
  4.`git reset --hard HEAD~1` (Undoing edit from push)  
  5.`git reser --soft HEAD~1` (Undoing commits)

## Collaboration
**Cloning**  
1.Go to [c9.io](www.c9,io)  
2.Open workspace  
3.In command line make sure you are in workspace  
4.Go to github of the other persons repo  
5.Click on green button that say > clone or download  
6.Make sure that link is on **SSH** not HTTPS  
7.Copy link `git@github.com:_username_/_repo name_.git`  
8.Type `git clone <copyed link>`

**Forking**  
1.Go to [c9.io](www.c9,io)  
2.Open workspace     
3.In command line make sure you are in workspace  
4.Go to github of the other persons repo  
5.Click on _Forking_ at top right corner  
6.Click on green button that say > clone or download  
7.Make sure that link is on **SSH** not HTTPS  
8.Copy link `git@github.com:_username_/_repo name_.git`   
9.cd into repo  
10.start your work

