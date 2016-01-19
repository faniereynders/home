> Please note: This document is still work in progress and solely serves as a draft set of (unofficial) guidelines may or may not be put in place.

# Contributing to WebApiProxy

Firstly, thank you for your participation in wanting to contribute to this awesome project! 

We'd love for you to contribute to our source code and to make WebApiProxy even better than it is
today! Like any OSS project we've compiled a few guidelines to help:

 - [Code of Conduct](#coc)
 - [Question or Problem?](#question)
 - [Issues and Bugs](#issue)
 - [Feature Requests](#feature)
 - [Submission Guidelines](#submit)
 - [Coding Rules](#rules)
 - [Commit Message Guidelines](#commit)
 - [Signing the CLA](#cla)
 - [Further Info](#info)

## <a name="coc"></a> Code of Conduct

> todo

## <a name="question"></a> Got a Question or Problem?

If you have questions about how to use WebApiProxy, please direct these to the [Gitter][gitter] group or even [StackOverflow][stackoverflow], be sure to tag the question or problem appropriately.

## <a name="issue"></a> Found an Issue?
If you find a bug in the source code or a mistake in the documentation, you can help us by
submitting an issue to our [GitHub Repository][github]. Even better you can submit a Pull Request
with a fix.

**Please see the Submission Guidelines below**.

## <a name="feature"></a> Want a Feature?
You can request a new feature by submitting an issue to our [GitHub Repository][github].  If you
would like to implement a new feature then consider what kind of change it is:

* **Major Changes** that you wish to contribute to the project should be discussed first on our
[Gitter][gitter] so that we can better coordinate our efforts, prevent
duplication of work, and help you to craft the change so that it is successfully accepted into the
project.
* **Small Changes** can be crafted and submitted to the [GitHub Repository][github] as a Pull Request.


## <a name="docs"></a> Want a Doc Fix?

> todo

## <a name="submit"></a> Submission Guidelines

### Submitting an Issue
Before you submit your issue search the archive, maybe your question was already answered.

If your issue appears to be a bug, and hasn't been reported, open a new issue.
Help us to maximize the effort we can spend fixing issues and adding new
features, by not reporting duplicate issues.  Providing the following information will increase the
chances of your issue being dealt with quickly:

* **Overview of the Issue** - if an error is being thrown a non-minified stack trace helps
* **Motivation for or Use Case** - explain why this is a bug for you
* **Which Component & Version(s)** - is it a regression?
* **Reproduce the Error** - provide a live example if possible or an unambiguous set of steps.
* **Related Issues** - has a similar issue been reported before?
* **Suggest a Fix** - if you can't fix the bug yourself, perhaps you can point to what might be
  causing the problem (line of code or commit)

Here is a great example of a well defined issue: [todo]

### Submitting a Pull Request
Before you submit your pull request consider the following guidelines:

* Search the appropriate repository for an open or closed Pull Request
  that relates to your submission. You don't want to duplicate effort.
* Please sign our [Contributor License Agreement (CLA)](#cla) before sending pull
  requests. ~~We cannot accept code without this.~~
* Make your changes in a new git branch:

     ```shell
     git checkout -b my-fix-branch master
     ```

* Create your patch, **including appropriate test cases**.
* Follow our [Coding Rules](#rules).
* Run unit tests.
* Commit your changes using a descriptive commit message that follows our
  [commit message conventions](#commit-message-format) and passes our commit message presubmit hook
  `validate-commit-msg.js`. Adherence to the [commit message conventions](#commit-message-format)
  is required because release notes are automatically generated from these messages.

     ```shell
     git commit -a
     ```
  Note: the optional commit `-a` command line option will automatically "add" and "rm" edited files.

* Build your changes locally to ensure all the tests pass:

    ```shell
    todo: example
    ```

* Push your branch to GitHub:

    ```shell
    git push origin my-fix-branch
    ```

* In GitHub, send a pull request to the `Dev` branch of the appropriate repository.
* If we suggest changes then:
  * Make the required updates.
  * Re-run the tests to make sure they are still passing.
  * Commit your changes to your branch (e.g. `my-fix-branch`).
  * Push the changes to your GitHub repository (this will update your Pull Request).

If the PR gets too outdated we may ask you to rebase and force push to update the PR:

    ```shell
    git rebase master -i
    git push origin my-fix-branch -f
    ```

*WARNING. Squashing or reverting commits and forced push thereafter may remove GitHub comments
on code that were previously made by you and others in your commits.*

That's it! Thank you for your contribution!

#### After your pull request is merged

After your pull request is merged, you can safely delete your branch and pull the changes
from the main (upstream) repository:

* Delete the remote branch on GitHub either through the GitHub web UI or your local shell as follows:

    ```shell
    git push origin --delete my-fix-branch
    ```

* Check out the master branch:

    ```shell
    git checkout master -f
    ```

* Delete the local branch:

    ```shell
    git branch -D my-fix-branch
    ```

* Update your master with the latest upstream version:

    ```shell
    git pull --ff upstream master
    ```

## <a name="rules"></a> Coding Rules
To ensure consistency throughout the source code, keep these rules in mind as you are working:

* All features or bug fixes **must be tested**.
* All public API methods **must be documented** as far as possible.
* With the exceptions listed below, we follow the following rules:
    * todo

## <a name="commit"></a> Git Commit Guidelines

We have very precise rules over how our git commit messages can be formatted.  This leads to **more
readable messages** that are easy to follow when looking through the **project history**.  But also,
we use the git commit messages to **generate the AngularJS change log**.

### Commit Message Format
Each commit message consists of a **header**, a **body** and a **footer**.  The header has a special
format that includes a **type**, a **scope** and a **subject**:

```
<type>(<scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

The **header** is mandatory and the **scope** of the header is optional.

Any line of the commit message cannot be longer 100 characters! This allows the message to be easier
to read on GitHub as well as in various git tools.

### Revert
If the commit reverts a previous commit, it should begin with `revert: `, followed by the header of the reverted commit. In the body it should say: `This reverts commit <hash>.`, where the hash is the SHA of the commit being reverted.

### Labels

> todo

### Scope
The scope could be anything specifying place of the commit change. [todo example]

### Subject
The subject contains succinct description of the change:

* use the imperative, present tense: "change" not "changed" nor "changes"
* don't capitalize first letter
* no dot (.) at the end

### Body
Just as in the **subject**, use the imperative, present tense: "change" not "changed" nor "changes".
The body should include the motivation for the change and contrast this with previous behavior.

### Footer
The footer should contain any information about **Breaking Changes** and is also the place to
reference GitHub issues that this commit **Closes**.

**Breaking Changes** should start with the word `BREAKING CHANGE:` with a space or two newlines. The rest of the commit message is then used for this.

A detailed explanation can be found in this [document][commit-message-format].

## <a name="cla"></a> Signing the CLA

> todo



*This guide was adopted from the original [AngularJs Contribution Guide](https://github.com/angular/angular.js/edit/master/CONTRIBUTING.md)*


[coc]: todo
[commit-message-format]: todo
[contribute]: todo
[contributing]: todo
[corporate-cla]: todo
[dev-doc]: todo
[github]: https://github.com/webapiproxy/home
[gitter]: https://gitter.im/webapiproxy
[individual-cla]: todo
[stackoverflow]: http://stackoverflow.com/questions/tagged/webapiproxy
[unit-testing]: todo

