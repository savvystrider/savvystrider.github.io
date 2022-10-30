# What is the architecture of Git?
Other version control system use a **two-tree architecture**. The two trees refer to the **repository** and the **working directory**:

``` mermaid
flowchart LR
    repository
    working
```

When we want to move files between the repository or the working directory, we "check out" copies from the repository into our working directory.

``` mermaid
stateDiagram-v2
    Repository --> Working
    Working --> Repository
```

***

##### Sources
- Skoglund, K. (2019). Git Essential Training: The Basics [Video]. LinkedIn Learning. https://www.linkedin.com/learning/git-essential-training-the-basics
- [Pro Git](hhttps://git-scm.com/book/en/v2)