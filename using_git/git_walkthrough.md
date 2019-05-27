# Git Walkthrough

For this walk-through, you'll want to open the Git shell. You can type the commands on the left and view the explanation on the right.

| **Command** | **Explanation** |
| :--- | :--- |
| git help | The only command you can't forget is help. This will help you find the other commands. |
| echo \# Products &gt;&gt; README.md | The first commit can be a README file with as little as one line summary of the project, or enough information about the project's first milestone. The broad topics can also include:   - Introduction  - Project description  - Project structure  - Coding conventions |
| git init | The git init command creates a new Git repository. It can be used to convert an existing, un-versioned project to a Git repository or initialize a new empty repository. This is the first command you’ll run in a new project.   git init creates a .git subdirectory in your project directory which all of the information git needs for your repository. The rest of an existing project is unchanged. |
| git add README.md |  Adds the README file to the index |
| git commit -m "first commit" | The first commit is usually called initial commit or First commit or something similar depending on your preferences. I prefer to get this out of the way and commit before adding many files. From then on I only work from a branch |
| git remote add origin https://github.com/dave45678/Products.git | git remote is used to add a new remote section called origin to our configuration. You can view he config file on windows using the type command. On unix this command is called cat. |
| type .git/config | The name origin is not special or unique. It's just the name that, by convention,  refers to the basis repository. |
| git push -u origin master | Any change that we had committed was local to our repository. Those changes don't exist on GitHub yet. You push your changes to GitHub with the push command. Here we're pushing to origin from master. |
| git status | status will show us the state of your index. It will show which files are presently staged. |
| git branch new\_feature | Now we add a branch from which to work. A branch is a good way to isolate development of a particular feature. Many developers build their  software one feature at a time. Test it. Make sure it works. Then merge the branch back into master and complete the process again.  |
| git checkout new\_feature | this is how you switch to the new\_feature branch |
| git branch | this is how you  view the local branches and note the one you’re on. In a little while you'll merge your new\_feature branch and delete it. |
| git status | status tells you the state of the index |
| "this is my shirts file"&gt;&gt;shirts.txt | create a new file for shirts |
| git add shirts.txt | add that to the index |
| git status | And see what happened |
| git commit -m "Add shirts to the product line" | now commit the shirts to the product line. |
| "this is the pants file"&gt;&gt;pants.txt | Add some pants |
| "this is the shoes file"&gt;&gt;shoes.txt | And some shoes |
| "this is the ties file"&gt;&gt;ties.txt | And some ties |
| mkdir outerwear | You want to add jackets, too. But I want to show you that you can work from sub-directories as well. Git will track all that. So, create a directory for outerwear and put the jackets in it. |
| "this is the jackets.txt"&gt;&gt;outerwear/jackets.txt | Next add the jackets to the outerwear directory |
| git add \*.txt | git add can add everything. It will find it all - even the sub-directory. |
| git commit -m "Add all the product text files" | commit the staged changes  to the project repository. |
| git log | git log shows the history of commits. It shows the history based on the current branch, unless you specify otherwise |
| git log master | This is Git log showing the history of the master branch. Git log has a number of other features as well. |
| git checkout master | Switch back to the master branch. |
| git status | Use status to see what's going on. None of the other files from new\_feature exist on master! |
| git ls-files | In the directory but it's part of the new\_feature branch, not master. |
| git merge new\_feature | merge the new\_feature branch to the current branch, master. |
| git branch -d new\_feature | Next delete the new\_feature branch. You’re done with that for now. |
| git branch | List the branches… no more new\_feature. |
| git push | Push your repository up to GitHub. If you're working with a team you would pull before you push so you could get their changes. |

