# Welcome to Vruh-Board Contributing Guide 

When contributing to this repository, please first discuss the change you wish to make via issue,
email, or any other method with the owners of this repository before making a change. 

Please note we have a [Code of Conduct](CodeofConduct.md), please follow it in all your interactions with the project.
## New contributor guide

To get an overview of the project, read the [README](README.md). Here are some resources to help you get started with open source contributions:

- [Finding ways to contribute to open source on GitHub](https://docs.github.com/en/get-started/exploring-projects-on-github/finding-ways-to-contribute-to-open-source-on-github)
- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
- [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow)
- [Collaborating with pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests)

### Make changes locally

1. [Install Git LFS](https://docs.github.com/en/github/managing-large-files/versioning-large-files/installing-git-large-file-storage).

2. Fork the repository.
- Using GitHub Desktop:
  - [Getting started with GitHub Desktop](https://docs.github.com/en/desktop/installing-and-configuring-github-desktop/getting-started-with-github-desktop) will guide you through setting up Desktop.
  - Once Desktop is set up, you can use it to [fork the repo](https://docs.github.com/en/desktop/contributing-and-collaborating-using-github-desktop/cloning-and-forking-repositories-from-github-desktop)!

- Using the command line:
  - [Fork the repo](https://docs.github.com/en/github/getting-started-with-github/fork-a-repo#fork-an-example-repository) so that you can make your changes without affecting the original project until you're ready to merge them.

- GitHub Codespaces:
  - [Fork, edit, and preview](https://docs.github.com/en/free-pro-team@latest/github/developing-online-with-codespaces/creating-a-codespace) using [GitHub Codespaces](https://github.com/features/codespaces) without having to install and run the project locally.

3. Install or update to **Node.js v16**.

4. Create a working branch and start with your changes!<br>

## 1. Commit Messages

- Use the `-m` flag only for minor changes. The message following the `-m` flag must be of the below format :

  > `<Verb>: <Action>`

  Verbs oftenly used are

  - add
  - feat
  - fix
  - refactor

  :white_check_mark: **Examples of valid messages:**

  - add: serialisers.py for users app
  - feat: validation
  - fix: functionality of authentication process
  - refactor: remove unwanted comments from src/auth.ts

  :x: **Examples of invalid messages:**

  - Idk why this is not working
  - Only ui bug fixes left
  - All changes done, ready for production :))

- Before opening a PR, make sure you squash all your commits into one single commit using `git rebase` (squash). Instead of having 50 commits that describe 1 feature implementation, there must be one commit that describes everything that has been done so far. You can read up about it [here](https://www.internalpointers.com/post/squash-commits-into-one-git).
  > NOTE: While squashing your commits to write a new one, do not make use of `-m` flag. In this case, a vim editor window shall open. Write a title for the commit within 50-70 characters, leave a line and add an understandable description.<br>
 
  Commit the changes once you are happy with them. See [Atom's contributing guide](https://github.com/atom/atom/blob/master/CONTRIBUTING.md#git-commit-messages) to know how to use emoji for commit messages.Once your changes are ready, don't forget to self review to speed up the review process:zap:.

## 2. Issues


#### Create a new issue

If you spot a problem with the docs, [search if an issue already exists](https://docs.github.com/en/github/searching-for-information-on-github/searching-on-github/searching-issues-and-pull-requests#search-by-the-title-body-or-comments). If a related issue doesn't exist, you can open a new issue using a relevant [issue form](https://github.com/github/docs/issues/new/choose). 

#### Solve an issue

Scan through our [existing issues](https://github.com/github/docs/issues) to find one that interests you. You can narrow down the search using `labels` as filters.


- Issues **MUST** be opened any time any of the following events occur:
  1. You want feature enhancements.
  2. You encounter bugs.
  3. Code refactoring is required.
  4. Test coverage should be increased.
- **Open issues with the given template only.**
- Feel free to label the issues appropriately.
- Do not remove the headings (questions in bold) while opening an issue with the given template. Simply append to it.

## 3. Branches and PRs

- No commits must be made to the `main`/`master` branch directly. The `main`/`master` branch shall only consist of the working code.
- Developers are expected to work on feature branches, and upon successful development and testing, a PR (pull request) must be opened to merge with `main`/`master`.
- A branch must be named as either as the feature being implemented, or the issue being fixed.

  :white_check_mark: **Examples of valid brach names:**

  - #123 (issue number)
  - OAuth (feature)
  - questionsUtils (functionality of the questions)

  :x: **Examples of invalid branch names**:

  - zeyan-testing
  - attemptToFixAuth
  - SomethingRandom
1. Ensure any install or build dependencies are removed before the end of the layer when doing a 
   build.
2. Update the README.md with details of changes to the interface, this includes new environment 
   variables, exposed ports, useful file locations and container parameters.
3. Increase the version numbers in any examples files and the README.md to the new version that this
   Pull Request would represent.
<br>
<br>
### Your PR is merged!

Congratulations :tada::tada: The [Vruh Board](README.md) team thanks you :sparkles:. 

Once your PR is merged, your contributions will be publicly visible on the [Vruh Board repository](https://github.com/dsc-iem/VruhBoard). <br>
<br>
## 4. Discussion Ethics

- Developers should be clear and concise while commenting on issues or PR reviews. If needed, one should provide visual reference or a code snippet for everyone involved to properly grasp the context.
- Everyone should be respectful of everyone's opinion. Any harsh/disrespectful language is **STRICTLY** prohibited and will not be tolerated under any circumstances.

## 5. Coding Ethics

- Developers are highly encouraged to use comments wherever necessary and make the code self documented.
- The project structure should be neat and organised. All folders and files should be organised semantically according to their functionality.
- The name of the folders and files should not be too long but should be as self explanatory as possible.
- Documentation shall **STRICTLY** have gender neutral terms. Instead of using "he/him" or "she/her", one should use "they/them" or "the user".

## 6. Coding Style Guidelines

Developers should aim to write clean, maintainable, scalable and testable code. If your code is not testable, that means, it's time to refactor it. The following guidelines might come in handy for this:

- Python: [Hitchiker's Guide to Python](https://docs.python-guide.org/writing/style/), [Google](https://github.com/google/styleguide/blob/gh-pages/pyguide.md)
- GoLang: [Effective-Go](https://golang.org/doc/effective_go.html)
- Django: [Django-Styleguide](https://github.com/HackSoftware/Django-Styleguide)
- JavaScript: [Airbnb](https://github.com/airbnb/javascript)
- React.JS: [Airbnb](https://github.com/airbnb/javascript/tree/master/react)
- Flutter/Dart: [Effective-Dart](https://dart.dev/guides/language/effective-dart)
- Kotlin: [Kotlin Conventions](https://kotlinlang.org/docs/reference/coding-conventions.html)
- Swift: [Swift Style Guide](https://github.com/github/swift-style-guide), [Google](https://google.github.io/swift/)
- Docker: [Dev Best Practices](https://docs.docker.com/develop/), [Dockerfile Best Practices](https://docs.docker.com/develop/develop-images/dockerfile_best-practices/)
