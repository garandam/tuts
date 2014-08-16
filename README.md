Tutorials
====

My collection of descriptions 

> "Documentation is like sex: when it is good, it is very, very good; and when it is bad, it is better than nothing"  
> Dick Brandon

### Table of Contents

  - Setup developer environment on Windows
  - ...

Setup developer environment on Windows
====

#### Tools to install
  - [GIT (Bash, GUI)](http://git-scm.com/downloads)
  - [Sublime-Text 3 (ST3)](http://www.sublimetext.com/)
  - [Virtual Box](https://www.virtualbox.org/wiki/Downloads)
  - [Vagrant](http://www.vagrantup.com/)
  - [PuTTY / PuTTYGen](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html)
  - [WinSCP](http://winscp.net/eng/index.php)
  - [7-zip](http://www.7-zip.de/)
  - [KeePass](http://keepass.info/)
  - (optional) [Fences](http://www.stardock.com/products/fences/)
  - (optional) [Dropbox](https://www.dropbox.com/)

## Install & Config

### GIT install
  ToDo ...

  - now you can use git-bash as cmd ;-)

  How to use GIT:
  - [Der einfache Einstieg](http://rogerdudler.github.io/git-guide/index.de.html)
  - [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/)

### SSH config
	$ cd ~
	$ mkdir .ssh 
	$ chmod 0700 .ssh/
	$ cd .ssh/
	$ vi config

	# Edit "config"-File
	Host github.com
	IdentityFile ~/.ssh/github.com/github
	
	Host vagrant
	HostName 127.0.0.1
	User vagrant
	Port 2222
	IdentityFile ~/.ssh/vagrant/vagrant

	[ESC] :wq

	### Try it
	$ clone thinks from github via SSH ;-)
	# or login to a vagrant-box
	$ ssh vagrant

#### Result .ssh-Tree
	.ssh/
	|-- github.com/
	|	|-- github
	|	└-- github.pub
	|-- vagrant/
	|	|-- vagrant
	|	└-- vagrant.pub
	|-- demo/
	|	|-- demo
	|	└-- demo.pub
	└-- config

### Sublime Text 3 (ST3)

#### [Download](http://www.sublimetext.com/) Sublime Text 3

#### Add Package Controll
ctrl + ! on Windows (Swiss-Layout) or  
View | Show Console  
Copy Python install code from [here.](https://sublime.wbond.net/installation)

#### Nice Packages
  SideBar Enhancment  
  Emmet  
  SublimeLinter

#### (optional) Sync-Config to Dropbox
  ToDo

#### (optional) subl alias
	$ cd ~
	$ vi .bashrc
	### add this line
	alias subl="/c/Program\ Files/Sublime\ Text\ 3/sublime_text.exe"
	[ESC] :wq

	### now you can use the "subl" alias on the cmd
	subl .
	subl file-Name
	subl folder-Name

	### Sample with & => with the "&" you can work on the cmd ;-)
	subl test.txt &



License
----

MIT
