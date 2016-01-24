# Vagrant CentOS 7 Project

This project contains the files created during the temporary CentOS 7 example showing finding and using a Vagrant box on the VagrantBox.es. Note, this project is deleted during the cours.

## Getting Started

This project is setup using the **Opscode** Ubuntu Vagrant box named **Opscode centos-7.0** which is the 64-bit version of the Ubuntu 14.04 LTS image packaged for VirtualBox.

### Setup

 * Go to the <http://vagrantbox.es> website
 * Search for "**opscode centos 7**"
 * Click the _copy_ button

### Commands

	# setup project folder
	cd ~
	mkdir -p projects/demo-centos-7
	cd projects/demo-centos-7
	# initalize Vagrant config
	vagrant box add centos-7.0 http://opscode-vm-bento.s3.amazonaws.com/vagrant/virtualbox/opscode_centos-7.0_chef-provisionerless.box
	vagrant box list
	vagrant init centos-7.0
	vagrant up
	vagrant status
	vagrant ssh
	# now inside VM
	exit
	# returned to host
	# delete project folder
	cd ..
	rm -rf demo-centos-

### Files

There will be a **Vagrantfile** that has the default configuration with the **Opscode centos-7.0** configured as per the vagrant init command.






