# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.hostname="jcrawshaw.qac.local"
  config.vm.box = "chad-thompson/ubuntu-trusty64-gui"
  config.vm.network "public_network", ip: "192.168.1.220"
  config.vm.synced_folder "shared", "/tmp/shared"
  
  config.vm.provider:virtualbox do |master|
	master.gui = true
	master.name = "Ansible Master"
	master.memory = "4096"
  end
  
end