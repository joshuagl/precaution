<!--
    Copyright 2019 VMware, Inc.
    SPDX-License-Identifier: BSD-2-Clause
-->

# Precaution

## Overview

Precaution provides simple, automated code reviews for GitHub projects by running code linters with a security focus on all pull requests.

Precaution currently supports analysis of:
* Go files via [Gosec](https://github.com/securego/gosec)
* JavaScript and TypeScript via [TSLint](https://github.com/palantir/tslint) and [tslint-config-security](https://github.com/webschik/tslint-config-security)
* Python files via [Bandit](https://github.com/PyCQA/bandit)

## Using Precaution

- [Initial setup](initial_setup.md)
- [False positives and how to handle them](false_positivies.md)

## Developing Precaution

- [Setting up a manual deployment](manual_deployment.md)
- [Debugging with VSCode](local_development.md)
- [Architecture](architecture.md)

## Community

* Fork us on GitHub: [vmware/precaution](https://github.com/vmware/precaution)
* File issues: [vmware/precaution/issues](https://github.com/vmware/precaution/issues)
* Chat with us on Slack: [VMware Code](https://code.vmware.com/web/code/join)]
