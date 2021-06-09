# -*- mode: ruby -*-
# vi: set ft=ruby :

#Vagrantfile API/syntax version. Dont touch unless you know what you're doing 
Vagrant.configure("2") do |config|
  
  config.vm.box = "chef/centos-6.5"

  config.vm.network "forward_port", guest: 80, host: 8080
  
  config.vb.guest.auto_update = false
  
  config.vm.provision "file", source: "~project/vagrant/file/git-config", destination: "~/.gitconfig"
  
  config.vm.provision "shell", path: "https://raw.githubusercontent.com/edcns07/vagrant/master/scripts/centos-lamp.sh"
  
  
end
