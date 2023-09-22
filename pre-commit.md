# [pre-commit](https://pre-commit.com/)


## Description

This hook is invoked by git commit, and can be bypassed with --no-verify option. It takes no parameter, and is invoked before obtaining the proposed commit log message and making a commit. Exiting with non-zero status from this script causes the git commit to abort.

## Useful links
- [pre-commit](https://pre-commit.com/)
- [pre-commit-hooks](https://pre-commit.com/hooks.html)
- [pre-commit-hooks GitHub](https://github.com/pre-commit/pre-commit-hooks)


## Installation

### 1. Install pre-commit with pip

```bash
pip install pre-commit
```

### 2. Create a pre-commit config file

```bash
touch .pre-commit-config.yaml
```

### 3. Add the following content to the config file

```yaml
repos:
- repo: https://github.com/pre-commit/pre-commit-hooks
  rev: v4.4.0
  hooks:
    - id: no-commit-to-branch
```

*This config file will prevent you from committing directly to the master/main branch.*

**If you want this in your first commit, consider add it now and commit it before you continue.**

### 4. Install the pre-commit hook

```bash
pre-commit install
```

*This will install the pre-commit hook to your .git/hooks folder.*

**Now you are ready to go!**

