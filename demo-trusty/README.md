# Vagrant Trusty-64 Project

This project contains the files created during the temporary **trusty-64** example showing finding and using a Vagrant box on the Hashicorp Atlas service. Note, this project is deleted during the course.

## Getting Started

This project is setup using the **Ubuntu** Vagrant box named **ubuntu/trusty64** which is the 64-bit version of the Ubuntu 14.04 LTS image packaged for VirtualBox.

### Setup

 * Go to the <http://atlas.hashicorp.com/boxes/search> website
 * Search for "**trusty64**"
 * Click on the Vagrant box name
 * Make note of the `vagrant init` command to be used later

### Commands

	# setup project folder
	cd ~
	mkdir -p projects/demo-trusty
	cd projects/demo-trusty
	# initalize Vagrant config
	vagrant init ubuntu/trusty64
	vagrant up
	vagrant status
	vagrant ssh
	# now inside VM
	exit
	# returned to host
	# delete project folder
	cd ..
	rm -rf demo-trusty

### Files

There will be a **Vagrantfile** that has the default configuration with the **ubuntu/trusty64** box configured as per the vagrant init command.






