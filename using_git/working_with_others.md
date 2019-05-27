# Working with Others

When working on a team one person will create a very basic project and a repository. Next they should check the basic project into the new repository on GitHub. Generally the basic project should consist on only one file: readme.md.

## Adding Collaborators

Before you can work on a team you must create a single repository for the team. Then from that repository add some collaborators. You can do this from the GitHub website by clicking on the repository. Then select **Settings**. Then select **Collaborators**. Enter the Collaborator's email or full name.

## Clone the project locally

Using git on your local computer, you can clone the other project to get a local copy:

```text
#git clone https://github.com/gitusername/gitrepositoryname
```

Now you can modify the files locally and even add or remove files. You should coordinate with your team mates so two people are not simultaneously working on the same file. When this happens you have to merge the two files and decide which changes to keep or discard.

When you are done editing you can push your changes back to the team's repository. Allways run `git pull` before adding files. That way you will get the latest version and minimize conflicts.

## Synchronize your local and remote repository

```text
#git pull
#git add .
#git commit -m "modified some file"
#git push origin master
```

## Your assignment

Working with one or two other people, create a simple project. Designate one person to create a repository and submit the project. Then you and any other teammates should follow the above commands to get comfortable working with Git as a team.

