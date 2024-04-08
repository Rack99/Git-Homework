# What is a pull request?
A pull request (PR) in Git serves as a proposal to merge changes made in one branch of a repository into another, typically from a feature branch into the main branch. Here’s how it works:

## Decentralized System:

Git operates as a completely decentralized system. The repository on platforms like GitHub or GitLab is no different from your local repository. When you want to contribute changes, you copy the code from the remote repository to your local repository and work on it there.

Pushing changes involves making commits and running git push, which updates the remote repository to sync with your local repo. However, this requires permission (usually via a password or SSH key).

## Pulling Changes:

When coworkers make changes and push them, you often run git pull to sync your local repo with the remote repository. But Git’s decentralization allows you to run git pull in reverse—from the server to your local repo. This concept forms the basis of pull requests.

## How Pull Requests Work:

A pull request is your way of telling the remote server (and its maintainers) that you have updated commits you’d like them to review and integrate into the remote repository. If they accept the changes, the remote repo runs git pull against your local repository, integrating the code without requiring your SSH key authorization.

Pull requests facilitate collaboration, code reviews, and the seamless integration of contributions.

## Open Source Collaboration:

Pull requests are crucial for open source projects. They allow any developer to contribute useful code. Project maintainers review pull requests, decide whether to integrate the code, and address any necessary fixes before merging.