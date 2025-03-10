---
title: Pull Requests
linkTitle: PRs
description: Gateway to the RAPIDS documentation content
type: docs
weight: 10
---

## Overview

Overview of creating a pull request for a RAPIDS project.

### See also

- [Issues]({{< relref "issues.md" >}})
- [Code Contributions]({{< relref "code.md" >}})
- [Changelog]({{< relref "../maintainers/changelog.md" >}})

## Create a pull request

Follow the steps
[here](https://help.github.com/articles/creating-a-pull-request/) to create a
draft pull request (PR) for the target repository.

Guidelines for managing forks and branches:
- Use a [fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/about-forks) of the upstream RAPIDS repository.
- On your fork, create a branch with a name describing the planned work.
  For example, `fix-documentation`.
- When opening the pull request, verify the target branch.
  By default, PRs target the next release branch.

Follow the format below for the title and description.

## Format a pull request

### Title

Pull request titles should be succinct and state how the PR addresses the issue.

- Use the present tense ("Add feature" not "Added feature")
- Use the imperative mood ("Move cursor to..." not "Moves cursor to...")

### Description

The description must start with `Closes #[issue number]`.
If the PR [addresses multiple issues](https://help.github.com/articles/closing-issues-using-keywords/#closing-multiple-issues), use an unordered list and repeat `Closes #[issue number]` for each issue.
For example:

```
- Closes #45
- Closes #60
```

The description should also detail the implementations, challenges, and solutions so reviewers can understand the approach.
Liberally reference related pull requests or related issues, especially if this pull request may affect them.

The description should provide any context not found in the issue description.

### Comments

All pull request comments and reviews must follow the [Code of Conduct]({{< relref "../maintainers/conduct.md" >}})

## Lifecycle

### Drafting and Testing

[Draft pull
requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests#draft-pull-requests)
should be opened while work is in progress. This will run continuous integration
(CI) without automatically requesting review. Once the pull request is ready, click "Ready for review" to get
feedback on the changes.

### Reviewing and Merging

Once the pull request is ready, open the draft and reviewers will be requested automatically.

All pull requests must pass continuous integration [status checks](https://help.github.com/articles/about-status-checks/).

Once approved, a pull request can be merged by an approved reviewer.
