# Introduction

Welcome! Thank you for considering contributing to the logo of the Rbanism community! We hope that you will find working
on this project to be an excellent exercise of your creativity and programming skills alike.

This guide aims to outline the general procedure potential contributors should follow for their work to be considered 
for integration into this repository. Though all contributions are wholeheartedly encouraged, and their authors will be 
assisted in their efforts by the Rbanism Core Team whenever necessary, it is of utmost importance to adhere to a certain
workflow in order to avoid miscommunication and increase productivity for everyone involved. Therefore, you are kindly 
asked to read this guide before contributing to this repository.

For any clarification or technical question regarding the contents of this guide, please contact Claudiu Forgaci.

# Quick Reference Guide

- [Submitting a Logo Generator](#submitting-a-logo-generator)
   <p> How to submit a logo generator. </p>
- [Proposing Changes to the Source Code](#proposing-changes-to-the-source-code)
   <p> How to propose a change to the source files of this repository. </p>

# Getting Started

## Code of Conduct

By contributing to this repository, you automatically become a valued member of our community. However, with great power
comes great responsibility! Therefore, we expect all members of the Rbanism community to adhere to our
[Code of Conduct](CODE-OF-CONDUCT.md).

## Prerequisites

This guide assumes that you have already installed R, RStudio, and Git in your system, and have set up your GitHub
account and local credentials. If you have not performed or are not sure that you have performed any of these steps,
please visit the [RStudio](https://posit.co/download/rstudio-desktop/) download page and see the GitHub guide on how to
[Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git).

# General Guidelines & Instructions

## Forking this Repository

### Creating your Fork

You can fork this repository by following
[these](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository) steps. You should copy only
the `main` branch so check the "Copy the `main` branch option" if this action has not already been performed
automatically.

### Cloning your Fork

You can clone your fork by following
[these](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository) steps.

Alternatively, you can create a new RStudio project directly from a version control platform by:

1. Clicking on `File > New Project...`.
    - A window titled "New Project Wizard" should appear. The remaining steps refer to it.
2. Clicking on `Version Control` and then `Git`.
3. Putting `https://github.com/YOUR-USERNAME/logo` as the repository URL in the corresponding text input field.
4. Filling in a unique and relevant project directory name and system path if this action has not already been performed
   automatically.
5. Clicking on `Create Project`.

The resulting project will itself be under version control, which allows you to interact with its online counterpart
using the `Git` tab on the upper right corner of the screen or the `Terminal` tab.

Note that if you decide to clone your fork programmatically, you can still open the resulting directory as an RStudio
project, and it should be set up correctly.

# Submitting a Logo Generator

A [tutorial](https://youtu.be/azR3VRPhQLM) on how to make a submission is to our logo generator challenge is also
available on YouTube.

## Prerequisites

It is assumed that you have already [forked this repository](#forking-this-repository).

## Preparing a Submission

Your submission should be a single [R Markdown](https://rmarkdown.rstudio.com/) notebook containing your name and a
brief explanation of how it works using a combination of text and short code snippets. In order to ensure uniformity
amongst all submissions, we kindly request you to adhere to the provided [template](submission.Rmd) and to not edit any
other file.

## Committing & Pushing the Submission

You can confirm your submission locally by staging and committing your version of `submission.Rmd`. You can do this by
executing `git add submission.Rmd`, `git commit -m "YOUR-MESSAGE"`, and `git push` in the Terminal tab this order. You
ought to write a descriptive commit message in either title or sentence case, preferably using fifty characters or
fewer. A commit message should start with an action verb in imperative, present mood.

## Creating a Pull Request

You can open a pull request (PR) from your fork by following
[these](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
steps. The title and description of your PR do not need to be overly detailed, since all relevant information should
already be included in `submission.Rmd`. However, you should
[request a review](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review)
from [Claudiu Forgaci](https://github.com/cforgaci), assign the PR to yourself, and label it using the provided
"submission" label.

For an example submission, please take a look at [this](https://github.com/Rbanism/logo/pull/1) PR.

# Proposing Changes to the Source Code

## Prerequisites

It is assumed that you have already [forked this repository](#forking-this-repository).

## Opening an Issue

You can open an issue regarding a proposed change to the source code of this repository by following
[these](https://docs.github.com/en/issues/tracking-your-work-with-issues/quickstart) steps. The title and description of
the issue should be as detailed as possible, unless the suggested amendment is completely obvious, such as a missing
licence or a typographical error. Moreover, make sure to assign the issue to
[Claudiu Forgaci](https://github.com/cforgaci) and yourself — if you are planning on working on it — and label it
accordingly.

If none of the available labels match the nature of your issue, please do not add one but submit a separate issue to
bring our attention to the matter.

[//]: # (TODO - Open a good example issue.)

## Committing & Pushing Changes

You can confirm your changes locally by staging and committing your version of the files that you have added or edited.
You can do this by executing `git add FILES`, where `FILES` is a space-separated list of relative system paths to said
files. Alternatively, if `FILES` is too long to type, you can use `git add .` to stage every file that appears in the
Git tab.

You can commit staged changes by running `git commit -m "YOUR-MESSAGE"`, and `git push` in the Terminal tab this order.
You ought to write a descriptive commit message in either title or sentence case, preferably using fifty characters or
fewer. A commit message should start with an action verb in imperative, present mood.

If your changes are too many to encompass in a single sentence, consider splitting them into smaller, thematically
similar commits, or adding a list of changes to your commit message. You can do this using the windows titled "RStudio:
Review Changes", which appears when clicking on the button with the green check mark in the upper left corner of the Git
tab. A long commit message should be composed of a title which adheres to the previously-mentioned guidelines, as well
as an unordered changelist, as follows:

```
YOUR-MESSAGE

- YOUR-CHANGE-1
- YOUR-CHANGE-2
- YOUR-CHANGE-3
.
.
.
```

Each change should be described by a sentence starting with an action verb in simple past tense.

[//]: # (TODO - Create a commit with a long commit message.)

## Creating a Pull Request

You can open a pull request (PR) from your fork by following
[these](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
steps. The title and description of your PR should be as detailed as possible unless the proposed changes are
immediately obvious, such as the addition of a licence or the amendment of a typographical error. In addition, you must
mention which issue your PR is related to in its title. Moreover, make sure to
[request a review](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review)
from [Claudiu Forgaci](https://github.com/cforgaci), assign the PR to yourself, and label it using the same label that
you used for the corresponding issue.

[//]: # (TODO - Open a good example issue.)

# Conclusion

Congratulations! You now know how to contribute not only to this repository, but any real open-source project using a
simplified, branch-less version of the
[fork-and-pull-request workflow](https://github.com/susam/gitpr/blob/master/README.md)!

# References

This guide references the following sources:

- The GitHub [guide](https://docs.github.com/en/get-started/quickstart/set-up-git) on setting up Git.
- The GitHub [guide](https://docs.github.com/en/issues/tracking-your-work-with-issues/quickstart) on submitting issues.
- The GitHub [guide](https://docs.github.com/en/get-started/quickstart/fork-a-repo) on forking a repository.
- The GitHub
  [guide](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)
  on opening a pull request from a fork.
- The GitHub
  [guide](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/requesting-a-pull-request-review)
  on requesting a pull request review.
- The Auth0 contribution [guide](https://github.com/auth0/open-source-template/blob/master/GENERAL-CONTRIBUTING.md).
