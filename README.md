# Manual Mac Setup

1. Change theme to dark 
	```
	System Preferences>General>Appearance>Dark
	```

2. [Install Homebrew](http://osxdaily.com/2018/03/07/how-install-homebrew-mac-os/)
	```
	/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
	```

3. [Terminal](https://www.freecodecamp.org/news/how-to-configure-your-macos-terminal-with-zsh-like-a-pro-c0ab3f3c1156/)
    - iTerm2
    	```
    	brew cask install iterm2
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

4. Spectacle 
	```
	brew cask install spectacle
	```
	- NB: Spectacle is no longer actively maintaned and (Rectangle)[https://github.com/rxhanson/Rectangle] is a recommended open-source alternative

5. Disable Siri 
	```
	System Preferences>Siri
	```

6. Install Itsycal 
	```
	brew cask install itsycal
	```
	- (E, MMMM d h:mm a) and replace system clock

7. Outlook
	- Change read behavior (Outlook>Preferences>Reading>Mark Mail As Read)