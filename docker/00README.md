```bash
# Install required software

brew cask install vagrant
brew cask install virtualbox
vagrant plugin install vagrant-parallels     # optional
brew install docker

# Create Vagrantfile

# Boot
vagrant up  # --or-- vagrant up --provider parallels
export DOCKER_HOST="tcp://`vagrant ssh-config | sed -n "s/[ ]*HostName[ ]*//gp"`:2375"

# If docker client and server versions don't match
DOCKER_API_VERSION=1.16 docker version
```
