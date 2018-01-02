Create various virtual machines using Vagrant.

# VirtualBox+Vagrant Installation on Centos 7#

```
##
## Step 1: First install VirtualBox dependencies.
##

$ yum -y install gcc dkms make qt libgomp patch
$ yum -y install kernel-headers kernel-devel binutils glibc-headers glibc-devel font-forge

$ mkdir -p /etc/yum.repos.d/; cd /etc/yum.repos.d/
$ wget http://download.virtualbox.org/virtualbox/rpm/rhel/virtualbox.repo

$ yum install -y VirtualBox-5.1
$ /usr/lib/virtualbox/vboxdrv.sh setup # In CentOS 7

##
## Step 2: Installing Vagrant on CentOS 7
##

$ yum -y install https://releases.hashicorp.com/vagrant/2.0.1/vagrant_2.0.1_x86_64.rpm

```


