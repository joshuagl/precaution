<!--
    Copyright 2019 VMware, Inc.
    SPDX-License-Identifier: BSD-2-Clause
-->

# Initial setup

## Run static code analysis tooling (recommended)

For best results, prior to using Precaution, it is recommended to run static code analysis tooling on the code base. That way the current code base does not contain known security issues.

The table below lists the languages supported by Precaution and the static analysis tools used by Precaution in support of the language. You should use the appropriate tool from the list for your initial scans before enabling Precaution.

| Language | Static analysis tool |
|---|---|
| Go | [Gosec](https://github.com/securego/gosec) |
| Python | [Bandit](https://github.com/PyCQA/bandit) |

## Setting up a Branch Protection Rule

By default, after Precaution is installed, it will not automatically prevent the merging of a pull request even if the check resulted in a failure status. 

![check_fails](./images/check_fails.png)


In order to allow Precaution to prevent pull requests from merging, do the following:

### 1. Create a pull request

You should create a pull request after the installation of Precaution in order to setup Precaution as a branch protection rule.

This pull request doesn't have to be merged.

### 2. Go to settings

![settings](./images/settings.png)


### 3. Choose branches

![branches](./images/branches.png)


### 4. Create a new branch protection rule 

![add_rule](./images/add_rule.png)


### 5. Setup the branch protection rule 

If you want to apply this rule to the master branch you will have to check the following options:

![branch_protection_rule.png](./images/branch_protection_rule.png)



Congratulations! Now Precaution will prevent the merging of a pull request if the check resulted in a failure status.
