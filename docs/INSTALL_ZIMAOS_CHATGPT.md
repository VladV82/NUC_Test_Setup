# Install ZimaOS ChatGPT

The project ships with a single helper script, `Fixdows`, which clones the
resources required for ZimaOS ChatGPT. This guide walks you through both the
scripted and manual installation options.

## 1. Prerequisites

- **Git** (required for the manual workflow).
- **GitHub CLI (`gh`)** if you want to run the helper script unchanged.
- A GitHub account with access to the repository `pistasjis/Fixdows2`.

## 2. Run the helper script (recommended)

1. Ensure the GitHub CLI is installed. On most Debian/Ubuntu systems:

   ```bash
   type gh >/dev/null 2>&1 || sudo apt install gh
   gh auth login
   ```

2. From the repository root, execute the script:

   ```bash
   bash Fixdows
   ```

   The script executes a single command, `gh repo clone pistasjis/Fixdows2`,
   which downloads the downstream installer repository into your current
   directory.

3. Change into the freshly cloned directory and follow its README or setup
   instructions to finish the ZimaOS ChatGPT installation.

## 3. Manual cloning (when `gh` is unavailable)

If you cannot install the GitHub CLI, replicate the script manually with Git:

```bash
git clone https://github.com/pistasjis/Fixdows2.git
cd Fixdows2
```

From there, follow the documentation provided in the cloned repository.

## 4. Troubleshooting

- **`gh: command not found`** – Install the GitHub CLI or use the manual cloning
  instructions above.
- **Authentication errors** – Ensure you have GitHub credentials with access to
  the downstream repository. For private repositories, authenticate via `gh auth
  login` or configure Git credentials for HTTPS cloning.
- **Network errors** – Retry the clone operation once connectivity is restored or
  consult your network administrator if outbound GitHub access is restricted.

With the repository in place, continue by running any setup scripts provided by
`pistasjis/Fixdows2` to complete the ZimaOS ChatGPT installation.
