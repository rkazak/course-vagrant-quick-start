# Vagrant Quick Start Project

The Vagrant Quick Start project will evolve through the Vagrant Quick Start course. Use the tags/releases feature in GitHub to see a version of this folder at a particular point in the course.

## Getting Started

The initial quick start project is setup using the **Hashicorp** Vagrant box named **hashicorp/precise64** which is the 64-bit version of the Ubuntu 12.x image packaged for Vagrant. If you have a 32-bit version, use **hashicorp/precise32** instead.

### Commands

	# setup project folder with Git SCM
	mkdir -p projects/vagrant-quickstart
	cd projects/vagrant-quickstart
	git init .
	# initalize with default Vagrant config
	vagrant --version
	vagrant init hashicorp/precise64
	vagrant up
	vagrant status
	vagrant ssh
	# now inside VM
	cd /vagrant
	exit
	# returned to host
	mate .gitignore # add .vagrant to contents
	# npp .gitignore (on Windows)
	# Clean up with Git
	git add .
	git commit -m "Initial Vagrant project files"

### Files

There will be a **Vagrantfile** that has the default configuration with the **hashicorp/precise64** (or 32-bit version) configured as per the vagrant init command.

Also, at the end of the quick start section, you should have a **.gitignore** file that will exclude any file or folder pattern (one per line) specified.





