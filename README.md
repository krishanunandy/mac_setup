# Manual Mac Setup

1. Change theme to dark 
	```
	System Preferences > General > Appearance > Dark
	```

2. [Install Homebrew](http://osxdaily.com/2018/03/07/how-install-homebrew-mac-os/)
	```
	/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	```

3. [Terminal](https://www.freecodecamp.org/news/how-to-configure-your-macos-terminal-with-zsh-like-a-pro-c0ab3f3c1156/)
    - iTerm2
    	```
    	brew install --cask iterm2
    	```
	- ZSH
		```
		brew install zsh
		```
    - Oh My Zsh!
    	```
    	sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
    	upgrade_oh_my_zsh
    	```
    - Powerlevel9k
    	```
    	git clone https://github.com/bhilburn/powerlevel9k.git ~/.oh-my-zsh/custom/themes/powerlevel9k
    	```
    	- In `~./zshrc` set `ZSH_THEME="powerlevel9k/powerlevel9k"` and update with `source ~/.zshrc`
    - Install powerline fonts
    	```
    	git clone https://github.com/powerline/fonts.git
		cd fonts
		./install.sh
		```
    	- Navigate to `iTerm2 > Preferences > Profiles > Text > Font > Inconsolata`
	- Set color theme
		- Download `https://github.com/mbadolato/iTerm2-Color-Schemes`
		- Navigate to `Preferences > Profiles > Colors > Color Presets` and import `Arthur` 
		- Set `Preferences > Profiles > Colors > Color Presets > Arthur`
	- Install plugins
		```
		git clone https://github.com/zsh-users/zsh-docker.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-docker
		```
		- Add plugin to the plugin section of `~/.zshrc`
		- Virtual environment
			```
			plugins=(virtualenv)
			POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS=(status virtualenv)
			```

4. Spectacle 
	```
	brew install --cask spectacle
	```
	- NB: Spectacle is no longer actively maintaned and [Rectangle](https://github.com/rxhanson/Rectangle) is a recommended open-source alternative

5. Disable Siri 
	```
	System Preferences > Siri
	```

6. Install Itsycal 
	```
	brew install --cask itsycal
	```
	- Set date/time format to `E, MMMM d h:mm a`
	- Replace system clock

7. Outlook
	- Change read behavior (`Outlook > Preferences > Reading > Mark Mail As Read`)

8. Install StatusClock from AppStore
	- Set UTC time

9. Install Statusfy
	```
	brew install --cask statusfy
	```