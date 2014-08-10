Tutorials
====

My collection of descriptions

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

#### Config

#### SSH
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
	--- github.com/
	-------------- github
	-------------- github.pub
	--- vagrant/
	----------- vagrant
	----------- vagrant.pub
	--- demo/
	-------- demo
	-------- demo.pub
	--- config

#### ST3



License
----

MIT
