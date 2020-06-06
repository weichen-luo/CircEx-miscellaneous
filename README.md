# CircEx-miscellaneous

## WSL (Allows Windows User to work on Linux)

### WSL Installation

Before you start, make sure your Windows 10 version is higher than `Windows 10 build 18342` <br>
Installation ref: https://ubuntu.com/wsl

1. Open **PowerShell** as Administrator and run this command:

   `Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux`

2. Download Ubuntu for WSL from the Microsoft Store, and run Ubuntu from the Start Menu and create your initial user. All following commands will be run in **Ubuntu**

3. Run `cd && sudo apt-get update && sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev xz-utils tk-dev python3-pip`

4. Run `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"` to install Homebrew

5. Run the following commands in `Next Steps` output message:

   - `sudo apt-get install build-essential`
   - the command under `Configure Homebrew in your /home/***/.profile by running`
   - the command under `Add Homebrew to your PATH`
   - `brew install gcc`

6. Generate a SSH key and add it to your GitHub account, reference:

   - Generate SSH key: https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key

7. Restart your Ubuntu terminal and run `cd` (now your working directory should look like `/home/alex`)

<!-- #### Workflow on WSL with Pycharm

1. Clone the project and navigate to the project directory in your Mac/Ubuntu terminal
2. Open it with PyCharm
   - For Windows, folder path should look like `\\wsl$\Ubuntu-20.04\home\alex\project_xxx`
3. Go to `Pycharm > Preferances > Project: xxx > Project Interpreter` click the cog and select `add`
   - For Mac, create virtual environment on your working directory
   - For Windows, select WSL, choose your Linux distribution (e.g. Ubuntu), and paste `/home/<username>/.pyenv/versions/3.6.6/bin/python` to Python Interpreter Path (Setup of Pyenv to be updated)
4. Go to `Pycharm > Preferances > Project: xxx > Project Structure` right click on your source code folders and tick sources -->

### Workflow on WSL with VS Code

Ref: https://code.visualstudio.com/docs/remote/wsl#_getting-started

1. Clone the project and navigate to the project directory in your Ubuntu terminal
2. Run `code .` to open VS Code

## Remote development (SSH) with VS Code

Ref: https://code.visualstudio.com/docs/remote/ssh#_getting-started

## Zsh (A handy alternative to Bash)

- For Mac and Linux (WSL), go to https://github.com/unixorn/zsh-quickstart-kit#os-specific-setup
- If you have zsh installed or configured previously, and above installation process causes an error, go to: https://github.com/unixorn/zsh-quickstart-kit#set-up-zgen-and-the-starter-kit

## GitHub workflow

1. Create new branch from master, name it with "bug-fix-xxx", "feature/xxx", or in a readable manner
2. When you finish your work, submit a pull request (PR) to merge your feature branch into master. If you want others to review your code, nominate a reviewer(s), and don't click `Merge pull request` yet. Ref: https://youtu.be/8fx-EaOUK2E?t=471
3. When you do coding peer review, leave comment on changed files if needed. When no further changes is required, merge pull request.

## How to write README file

- https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax

## Handy VS Code plugins

- Prettier (code formatter for several common languages)
- GitLens (better GitHub plugins)
-

Submit a PR if you have any update to this guide.
