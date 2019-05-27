# Git Commands

From Eclipse locate the Project directory by right-clicking on the project folder and then selecting Properties from the menu.

1. sign into github.com
2. create new repository: MyFirstProject
3. open the terminal on your pc and change to the project directory
4. run the following commands at the prompt 

   ```bash
   git init
   git remote add origin https://dave45678@github.com/dave45678/MyFirstProject
   git config -l
   git add --all
   git commit -m "commit message"
   git push -u origin master
   git status
   ```

The project files should now be on github

After you make changes to your project:

```bash
git add --all
git commit -m "commit message"
git push
git status
```

Notes: if origin already exists then use

```bash
git remote set-url origin https://dave45678@github.com/dave45678/MyFirstProject (Links to an external site.)
```

You can create a file in your project directory called `.gitignore`

You can copy an example of .gitignore from [http://bit.ly/GitIgnore](http://bit.ly/GitIgnore) \(Links to an external site.\) and use that

For more details on creating .gitignore see [https://help.github.com/articles/ignoring-files/](https://help.github.com/articles/ignoring-files/) \(Links to an external site.\)

