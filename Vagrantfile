# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define :ubuntu do |cfg|
    cfg.vm.box = "ubuntu/trusty64"
    cfg.vm.box_url = "https://vagrantcloud.com/ubuntu/boxes/trusty64"
    cfg.vm.hostname = "ubuntu"
  end
  config.vm.define :docker do |cfg|
    cfg.vm.box = "sennerholm/boot2docker1_6"
    cfg.vm.box_url = "https://dl.dropboxusercontent.com/u/6816236/boot2docker_virtualbox1.6.0.box"
    cfg.vm.synced_folder "docker", "/docker"
  end
end
