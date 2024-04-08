# What is a conflict and how to solve it?
A conflict occurs when there are conflicting changes between different branches or commits that Git cannot automatically resolve. Conflicts typically arise during the process of merging branches or applying changes from one branch to another, such as during a pull request or when using commands like git merge or git rebase.

Conflicts can occur when:

- *Two or more branches have changes in the same part of a file:* Git cannot determine which change should take precedence, so it marks the file as conflicted.

- *A file was deleted in one branch and modified in another:* Git cannot determine whether to keep the modifications or delete the file.

- *A file was renamed in one branch and modified in another:* Git cannot determine how to apply the changes to the renamed file.

To resolve conflicts in Git, you need to follow these steps:

- Identify the conflicted files: Git will inform you which files have conflicts after you attempt to merge or apply changes.

- Open the conflicted files in your code editor: Git will mark the conflicted sections within the files, indicating the conflicting changes.

- Manually resolve the conflicts: Review the conflicting sections in the files and decide how to resolve them. You can choose to keep one version of the change, combine the changes, or discard one of the changes altogether. Make the necessary modifications directly in the conflicted files.

- Mark the conflicts as resolved: After resolving the conflicts in the conflicted files, save the changes in your code editor.

- Stage the resolved files: Use the git add command to stage the resolved files with the conflicts.

- Complete the merge or rebase operation: Once all conflicts are resolved and staged, you can proceed to complete the merge or rebase operation using the git merge --continue or git rebase --continue command.

- Commit the merge or rebase: After resolving conflicts and completing the merge or rebase operation, you need to commit the changes using git commit. This creates a new commit that includes the resolved conflicts.