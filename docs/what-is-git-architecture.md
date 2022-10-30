## What is a two-tree architecture?
Other version control systems use a **two-tree architecture**. The two trees refer to the **repository** and the **working directory**:

``` mermaid
flowchart LR
    A[repository]
    B[working]
```

You "check out" files from the repository and edit them within your working directory:

``` mermaid
stateDiagram-v2
    repository --> working: checkout
    working --> repository: commit
```

After those changes are made, you **commit** the changes back to the repository.

## What is a three-tree architecture?
Git uses a three-tree architecture. It has:

- A **repository** that's tracked by Git.
- A **working directory** that contains changes that may not be tracked by Git yet.
- A **staging index** in between the repository and working directory that contains changes we plan to commit to the repository.

``` mermaid
flowchart LR
    A[repository]
    B[staging index]
    C[working]
```
In Git, you have a copy of the repository in your working directory where you can edit files. When you're ready for Git to start tracking your changes, you add files to the staging index. Then, you commit your changes to the repository along with a message.

***

##### Sources
- Skoglund, K. (2019). Git Essential Training: The Basics [Video]. LinkedIn Learning. https://www.linkedin.com/learning/git-essential-training-the-basics
- [Pro Git](https://git-scm.com/book/en/v2)