# Docs

Open documentation on how Squeeble develops projects and creates corresponding documents for such projects. In this document we will go over the guidlines of different disciplines. 

## Table of Contents

- [Git](#git)
  - [What is Git](#what-is-git?)
  - [Why GitHub](#why-do-we-use-Git-/-GitHub?)
  - [Commits](#commits)
    - [\<type> Why we use it](#common-prefixes-for-type)
    - [\<type> Prefixes](#common-prefixes-for-type)
    - [\<code> Why we use it](#why-we-use-code:)
    - [\<init> Why we use it](#the-use-of-an-init-word-of-the-description)
    - [\<init> Prefixes](#common-prefixes-for-init)
  - [Branching](#branching)
  - [Issues](#issues)

- [MarkDown](#markdown)
  - What is Markdown
  - Why Markdown files
  - Linking within a file
  - Linking outside a file

## Git

### What is git?  
Git is a [distributed version-control][g-1] system for tracking changes in [source code][g-2] during [software development][g-3]. It is designed for coordinating work among [programmers][g-4], but it can be used to track changes in any set of [files][g-5]. Its goals include speed, [data integrity][g-6], and support for distributed, non-linear workflows. Read more on [wikipedia][g-7]

### Why do we use Git / GitHub?  
We use GitHub for version control. Git simplifies the process of working with other people and makes it easy to collaborate on projects. Team members can work on files and easily merge their changes in with the master branch of the project.

### Commits

Commiting and keeping the commit history clear is importend. Here we go over our conventions and why we commit the way we do.

The commit message should be structured as follows:
```
<type>|<code>: <init><description>

[optional body]

[optional footer(s)]
```

- [\<type> Why we use it](#common-prefixes-for-type)
- [\<type> Prefixes](#common-prefixes-for-type)
- [\<code> Why we use it](#why-we-use-code:)
- [\<init> Why we use it](#the-use-of-an-init-word-of-the-description)
- [\<init> Prefixes](#common-prefixes-for-init)

#### Common prefixes for `<type>`:
>- Issue: A bug fix
>- Feat: A new feature
>- Docs: Documentation changes
>- Test: Adding missing or correcting existing tests
>- CICD: Changes to our CI configuration files and scripts
>- Perf: A code change that improves performance
>- Refactor: A code change that neither fixes a bug nor adds a feature
>- Style: Changes to software where the interface changes
>- Lint: Changes that do not affect the meaning of the code (linting)
>- Vendor: Bumping a (dev)dependency like node, express or electron
>- Revert: Reverting to a previous commit or merche

#### Why we use `<code>`:
>We make use of a `<code>` to refer to issues numbers and feature codes.
We prefix these codes with an hashtag with the corresponding code like this: `#123`. We do this since you might work on a new feature with the code `#456` and while working on this feature you encounter a bug that needs to be fixed before you can continue on the feature. Lets say that the bug is already know and not an high prio and has the code `#444`. You can now keep working in your feature branch without creating a branch for the bug if it did not existed. When there is an other project tool in use we will write the code with 

#### The use of an `<init>` word before the `<description>`
> We want `<description>` to be a logical sentence and by prefixing the first word (`<init>`) of the description you will write automatic a sentence that corresponse with what you have done.

#### Common prefixes for `<init>`:
>- Updated: When you updated an existing peace of code
>- Upgraded: When you updated a (dev)dependency
>- Fixed: When you fixed or corrected a typo or issue
>- Added: When you add a new feature or test

### Branching

### Issues

[g-1]: https://en.wikipedia.org/wiki/Distributed_version_control
[g-2]: https://en.wikipedia.org/wiki/Source_code
[g-3]: https://en.wikipedia.org/wiki/Software_development
[g-4]: https://en.wikipedia.org/wiki/Programmer
[g-5]: https://en.wikipedia.org/wiki/Computer_file
[g-6]: https://en.wikipedia.org/wiki/Data_integrity
[g-7]: https://en.wikipedia.org/wiki/Git

## Markdown
