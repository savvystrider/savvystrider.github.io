# How do I write good commit messages in Git?

Previously, we learned that we have to follow a process with Git:

1. First, we make changes.
2. Then, we [add](how-to-add-files-in-git.md) our changes.
3. Then, we [commit](how-to-commit-changes-in-git.md) our changes.
4. Finally, we add a **commit message**.

Some general guidelines for writing good commit messages:

- At the very least, explain *why* the commit was made and *what* the commit is supposed to do.
- Write a short, single-line summary that's less than 50 characters.
    -  You can follow this up with a blank line and a more complete description (optional).
- Write messages in present tense. Commit messages are labels for future use, so avoid using past tense.
    - `Fixes a bug`, not `fixed a bug`.
- Use asterisks (`*`) or hyphens (`-`) for bullet points.
- You can add, or start with, a tracking number from bugs or support requests.
- Be clear and descriptive.
- Commit messages are part of a permanent log. Don't include any information that doesn't belong.

!!! info

    The text up to the first blank line in a commit message is treated as the commit title, and that title is used throughout Git.



***

##### Sources
- Skoglund, K. (2019). Git Essential Training: The Basics [Video]. LinkedIn Learning. https://www.linkedin.com/learning/git-essential-training-the-basics
- [Pro Git](https://git-scm.com/book/en/v2)