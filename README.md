#Quick Start Using Homebrew on Mac OS X
> **Written 2016-01-01 by [@mikeschinkel](http://twitter.com/mikeschinkel)**

Homebrew is a [**Package Manager**](https://en.wikipedia.org/wiki/Package_manager) for Mac OS X similar to what you'll find for Linux.

According to Wikipedia a Package Manager is: 

> _"A software tool that automates the process of installing, upgrading, configuring, and removing computer programs for a computer's operating system in a consistent manner."_

Thus HomeBrew is: 

> _A command line tool that allows you to easily download and install other software packages for your Mac in a simple and easy to learn commands in Terminal._

##Installing Homebrew

To install Homebrew on Mac OS X run:
	
	ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"


##Running Diagnostics

After installing you'll want to run diagnostics and **attempt to fix any of the errors or warnings** _(Google is your friend here.)_ Note fixing the warnings might break over software you have installed but using Homebrew to reinstall the broken software will resolve most issues:
	
	brew doctor

Once _"Your system is ready to brew"_ you can start installing packages.

##Installing Packages
Installing a package is as simple as typing `brew install <package_name>`.  If you are a web developer some of the packages you might want to install are here _(unless you already have them installed):_

	brew install git 
	brew install wget 
	brew install node
	brew install npm
	brew install iterm2

**Hint:** Definitely switch to using [**iTerm2**](https://www.iterm2.com/) instead of the default OS X terminal program as soon as you install it.	

##Finding Packages
To discover packages simply search to list all available packages:

	brew search
	
You can also visit several websites that provide more information about available packages:

- [**Search Brew**](http://searchbrew.com/)
- [**Braumeister**](http://braumeister.org/)
- [**Homebrew Formulas on GitHub**](https://github.com/Homebrew/homebrew/tree/master/Library/Formula)


##Updating Homebrew
Homebrew is continuously being updated to its best to update and then run the doctor prior to using another other Homebrew commands if you have not recently done so:

	brew update
	brew doctor

##Adding Casks for Applications
You will probably also want to install the Homebrew _"Casks"_ which can extends Homebrew to allow it to install OS X applications and large binaries in addition to command line tools:


	brew tap caskroom/cask

##Finding Applications in Casks
Once you have Caskroom tapped you can find applications with search. 

For example if you where looking for Google's Chrome:


	$ brew cask search chrome
	==> Partial matches
	chrome-devtools				epichrome
	chrome-remote-desktop-host	google-chrome
	
If you'd like a quick gander at the over 2500 Casks available from [**Caskroom.io**](http://caskroom.io/) as of this writing [**click here**](cask-list.txt).


##Installing Applications from Casks
To install Google's Chrome _(although you probably already have it!):_

	brew cask install google-chrome
	
Another application you might not have that **a software developer definitely should be using** is Vagrant:

	brew cask install vagrant
	
If you are not familiar with it you can [**learn more about Vagrant here**](https://github.com/thecodersguild/learning-vagrant-for-wordpress).


##More about Homebrew and Casks
Now that you've finished your quick start of Homebrew you can start your journey to learn more about Homebrew and Caskroom here, respectively:

- [**Homebrew Docs**](https://github.com/Homebrew/homebrew/tree/master/share/doc/homebrew#readme)
- [**How to Use Homebrew-Cask**](https://github.com/caskroom/homebrew-cask/blob/master/USAGE.md)
