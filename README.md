# best-practices
This repository serves as a guide to best practices for software development and team collaboration.

### Below are some industry standards advisable to follow -

In a typical Git workflow, the "main" branch contains the latest stable version of the project. It's not advisable to directly add changes to the "main" branch. Instead, we use the "release" branch, which has tested code waiting to go live. Only after deploying the "release" branch should it's changes be merged into the "main" branch.

The "feature" branch is where we develop new features. It's always created from the "main" branch and is dedicated to feature-related work only. Before merging into the "release" branch, we must test the changes made in the "feature" branch and ensure that only code related to the feature is present in the "feature" branch and no extra code.

After all features are developed, the new changes from all "feature" branches are merged into the "release" branch.

For clear code, it's important to have good comments and formatting. When writing commit messages, use the present tense, like "Add feature to the app," instead of "Added feature to the app" or "Adding feature to the app."

In the "release" branch, keep things neat by avoiding print statements or commented-out code. And remember, never put sensitive information like API keys or passwords in the code.
