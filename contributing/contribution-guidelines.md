---
description: How to contribute to Nuclear
---

# Contribution guidelines

## Contributing to Nuclear

There are many ways to contribute to the Nuclear project: logging bugs, submitting pull requests, reporting issues, creating suggestions, and many others.

After cloning and building the repo, check out the [issues list](https://github.com/nukeop/nuclear/issues). Issues labeled `good first issue` are good candidates to pick up if you are contributing for the first time. If you are contributing significant changes, please discuss it in the issue first before starting to work on it.

### Before your changes can be merged

We treat code quality seriously, and while we're open to helping out new contributors, we also need to ensure that the contributions meet our standards.

Before you commit your code:

* Run linter \(`npm run lint:fix` in project root\) to format the code and automatically detect coding style issues, some of which can be automatically fixed
* Run tests and try to build the project \(`npm test` in project root\) to make sure that all tests pass and the project can be built with your changes
* If you're fixing a bug, or adding a new functionality, please create tests covering your changes. Look at the existing tests in each package or ask us on Github or Discord if you're unsure how to do it. We have automated test coverage checks for pull requests, and require code coverage to **never decrease.** It's fine if your pull request fails this check initially, but **coverage needs to at least stay the same for the PR to be merged**.
* If you're adding visual components in the `ui` package, please create snapshot tests for them. Most components there already have snapshot tests, take a look at them to see how they should look. Typically we will want the snapshots to cover all the different states the component can be in, and be filled with some example content.
* Add new visual components to Storybook \(`*.stories.tsx` files\). It's nice if you can also show us some screenshots in the pull request for reference.



