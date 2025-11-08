# NUC Test Setup

This repository contains helper assets that make it easier to set up the
**ZimaOS ChatGPT** experience on a new device. The primary entry point is the
`Fixdows` script located at the project root, which automates the cloning of the
downstream resources required for the installation.

## Getting started

If you just want the short version, run the following from the project root:

```bash
bash Fixdows
```

The script expects the [GitHub CLI](https://cli.github.com) to be available. If
`gh` is not installed, or if you prefer to avoid the additional dependency,
check out the [detailed installation instructions](docs/INSTALL_ZIMAOS_CHATGPT.md)
for a manual workflow that only requires Git.