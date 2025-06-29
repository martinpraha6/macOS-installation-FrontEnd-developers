# macOS installation tips for FrontEnd developers

You are the FrontEnd developer and you bought a new Mac. So, inspire and follow this instructions. If you have an idea to improve this, just create a Pull request. Thank you.

## System

1.  macOS

    - At first check if your system is up to date.

    - Install **Xcode** from the **AppStore**

2.  Terminal

    `xcode-select --version` If the result is not a version number, install the tools with this command: `xcode-select --install`

        sudo xcode-select -s /Applications/Xcode.app/Contents/Developer

    `brew --version` If you don’t see a version number, install Homebrew with this command:

        /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

    Zshell & the framework for Zsh configuration (optional) [Oh My ZSH!](https://ohmyz.sh)

        brew install zsh zsh-completions

        chsh -s /bin/zsh

        sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

    Open `~/.zshrc` and add some plugins e.g. `plugins=(git yarn npm)`

## Developer environment

1.  Git

        brew install git

2.  [NVM](https://github.com/nvm-sh/nvm?tab=readme-ov-file#install--update-script)

        wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash

        export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"
        [ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"

    Get a version list:

        nvm ls-remote

    Install a specific version:

    `nvm install <version>` e.g.: `nvm install 22`

3.  [Watchman](https://facebook.github.io/watchman/)

        brew install watchman

4.  Show hidden files in `Finder` (macOS)

    Open `Terminal` and launch:

    - `defaults write com.apple.finder AppleShowAllFiles NO`
    - `killall Finder /System/Library/CoreServices/Finder.app`

5.  Get all up to date

        brew update && brew upgrade && brew cleanup && brew doctor

## Developer tools

1.  IDE

        brew install visual-studio-code

    Set Visual Studio Code as your core editor:

    - Launch VS Code

    - Open the Command Palette `⇧⌘P` and type `shell command` to find the `Shell Command: Install 'code' command in PATH` command and run it

    - Open `Terminal` and run a the command `git config --global core.editor "code --wait"`

2.  Setting up Apple Silicon Macs for using package node-gyp

    - Configure node-gyp `export CXXFLAGS="-stdlib=libc++"`

    - Install node-gyp `npm install -g node-gyp`

3.  Browsers

        brew install google-chrome

        brew install firefox

## Communication

- [Discord](https://discord.com/download)

- [Skype](https://www.skype.com/cs/)

- [Skype for business](https://products.office.com/cs-cz/skype-for-business/download-app)

- [Slack](https://slack.com/intl/en-cz/)

- [Teams](https://www.microsoft.com/cs-cz/microsoft-teams/download-app)

- [TeamViewer](https://www.teamviewer.com/)

- [Zoom](https://zoom.us)
