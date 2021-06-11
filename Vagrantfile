# -*- mode: ruby -*-
# vi: set ft=ruby :

#Vagrantfile API/syntax version. Dont touch unless you know what you're doing 
 Vagrant.configure("2") do |config|
  config.vm.box = "bento/centos-7"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  config.vm.box_check_update = false
  config.vm.provision "file", source: "~/projects/vagrant/files/git-config", destination: "~/.gitconfig"
  config.vm.provision "shell", path: "https://raw.githubusercontent.com/edcns07/vagrant/master/scripts/centos7.9-lamp.sh"
end
