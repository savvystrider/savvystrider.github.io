# How do I configure Git?
After you install Git, you can configure settings in three different ways/locations:

- System level
- User level
- Project level

## System level configuration
You can configure system-wide settings with the following command:

`git config --system`

This will set configuration for all users and their repositories. You may need admin privileges to configure these settings.

## User level configuration
You can configure settings for specific users with the following command:

`git config --global`

This will set configurations for specific users and their repositories.

## Project level configuration
You can configure settings for a specific project by entering the project directory and running the following command:

`git config`

## First-time configuration
After you have installed Git, make sure to configure these settings.

### Configure user name and email address
In the command line, you can set your user name and email for Git:

`git config --global user.name "username"`
`git config --global user.email "email@example.com"`

This is important because a major part of the Git workflow is making "commits" and each commit needs this information.

### Configure your preferred text editor
You can configure the default text editor you want to use with Git. For example, if you'd like to set Visual Studio Code as your default text editor, just run the following command:

`git config --global core.editor "code --wait"`

You can find a full list of options [here](https://git-scm.com/book/en/v2/Appendix-C%3A-Git-Commands-Setup-and-Config#ch_core_editor).

### Configure color UI
Since Git utilizes command-line options, you may want to configure settings to display color. This should be enabled by default. You can confirm by running the following command:

`git config --global color.ui`

If the output is `True`, then it's installed. If the output is `False`, then you can enable color by using the following command:

`git config --global color.ui true`

Naturally, you can also turn off color UI with a similar command:

`git config --global color.ui false`

### List configurations
You can view a full list of your configurations by using the following command:

`git config --list`

To view individual configurations in the command line, use the following command:

`git config --global user.name`
`git config --global user.email`

*[UI]: User interface

***

##### Sources
- Skoglund, K. (2019). Git Essential Training: The Basics [Video]. LinkedIn Learning. https://www.linkedin.com/learning/git-essential-training-the-basics
- [Git](https://git-scm.com/)