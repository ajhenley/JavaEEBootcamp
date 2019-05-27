# Publishing your repository

## What is a repository?

A repository is a storage space where you can access your project, its files, and all the versions of its files that Git saves.

## Create an empty repository on GitHub

Before you can push your local repository to GitHub you first need to create an empty repository.

When you browse to your GitHub account you can click on the new repository button. The button looks like a plus sign and is found at the top right of the website.

Alternatively, you can simply browse to [https://github.com/new](https://github.com/new) \(Links to an external site.\)

Fill in the name your repository and click the large green button at the bottom of the page to finish the process of creating it. Your repository will be located at [https://github.com/{your](https://github.com/{your) **GitHub user name}/MyNewRepository**

## Pushing your local repository to GitHub

Now that you have a repository you can go back to your PC and push your existing repository to the one you just created. Make sure you have configured your commit author and email.

Next, you need to tell your local version of Git about the remote repository. Your local branch is called **master**. Your remote branch is called **origin**.

You do this by typing:  
 `git remote add origin https://github.com/<your GitHub user name>/Products`

The `git remote` command will add a new remote section called origin to our configuration.

View the git configuration with `git config --list` to check if your remote repository is initialized.

Running `git remote` without any arguments will show you the remote repository aliases.

If you run the command with the -v option, as `git remote -v`, you can see the actual URL for each alias.

