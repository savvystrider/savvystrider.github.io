# What is Git?

**Git** is a distributed version control tool that does not require a single master repository for all users. It is open-source software that keeps track of changes, especially text changes, to files and directories. With Git, you can compare old and new versions of files.

Its competitors include:

- Subversion
- CVS
- Perforce
- ClearCase
- Mercurial

!!! info

    Git was created in 2005 by Linus Torvalds, the creator of Linux.

## What is distributed version control?
In a central code repository model, source code is stored in one central location. Code is then checked out from this master repository.

Git uses **distributed version control**. Different users maintain their own local repositories instead of checking it out from the master repository. This means THERE IS NO CENTRAL REPOSITORY.

Changes are stored as *change sets*, or patches. Git tracks the *changes* to documents, not the versions of documents. These change sets can be exchanged between repositories.

There are many working copies, each with their own combination of change sets. This ensures that there is no single point of failure in case a server goes down.

If you've never used Git, or a distributed version control system, before, then the in's and out's can seem unfamiliar. Git utilizes the command line instead of a standard GUI; however, graphical user interface options are available.

## How do I know if Git is already installed on my computer?
Open up the command line on your terminal and run the following command:

`git --version`

Do you see a response this like this?

`git version 2.37.3.windows.1`

If not, then you will have to install Git.

## Are Git and GitHub the same thing?
Nope! [More on that later](what-is-github.md)...

***

##### Sources
- Skoglund, K. (2019). Git Essential Training: The Basics [Video]. LinkedIn Learning. https://www.linkedin.com/learning/git-essential-training-the-basics
- [Pro Git](https://git-scm.com/book/en/v2)