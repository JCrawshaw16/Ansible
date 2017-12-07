# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "chad-thompson/ubuntu-trusty64-gui"
  config.vm.synced_folder "shared", "/tmp/shared"
  
  config.vm.define "ansiMasterDG" do |master|
	master.vm.hostname = "ansiMasterDG.qac.local"
	master.vm.network "public_network", ip:"192.168.1.18"
  end
  
   config.vm.define "ansiAgentDG" do |agent|
	agent.vm.hostname = "ansiAgentDG.qac.local"
	agent.vm.network "public_network", ip:"192.168.1.19"
  end
  
end