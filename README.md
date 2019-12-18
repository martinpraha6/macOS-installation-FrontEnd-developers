macOS installation tips for FrontEnd developers
===

You are the FrontEnd developer and you bought a new Mac. So, inspire and follow this instructions. If you have an idea to improve this, just create a Pull request. Thank you.

System
---

1. macOS

	- At first check if your system is up to date.

	- Install **Xcode** from the **AppStore**

2. Terminal

	`xcode-select --version` If the result is not a version number, install the tools with this command: `xcode-select --install`

	`sudo xcode-select -s /Applications/Xcode.app/Contents/Developer`

	`brew --version` If you don’t see a version number, install Homebrew with this command:

		/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Zshell & the framework for Zsh configuration (optional) [Oh My ZSH!](https://ohmyz.sh)

		brew install zsh zsh-completions
		chsh -s /bin/zsh
		sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"

Open  **~/.zshrc** and add some plugins `plugins=(git yarn docker npm)`

Developer environment
---

1. Node

	`node --version` If not, install it with Homebrew: `brew install node`

Check if it was installed properly:

	node --version
	npm --version

2. Yarn

	`brew install yarn`

3. Git

	`git --version` If not, install it with Homebrew: `brew install git`
	`git --version`

4. Get all up to date

	`brew update && brew upgrade && brew cleanup && brew doctor`

5. [Watchman](https://facebook.github.io/watchman/)

	`brew install watchman`

6. Docker

Download and install [Docker](https://www.docker.com/)

Developer tools
---

1. IDE

	`brew cask install visual-studio-code`

2. Browsers

	`brew cask install google-chrome`

	`brew cask install firefox`

3. Postman

	`brew cask install postman`

Communication
---

* [Slack](https://slack.com/intl/en-cz/)

* [TeamViewer](https://www.teamviewer.com/)

* [Skype](https://www.skype.com/cs/)

* [Skype for business](https://products.office.com/cs-cz/skype-for-business/download-app)

* [Zoom](https://zoom.us)
