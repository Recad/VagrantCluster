# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  

  config.vm.define "master" do |master|
   
    master.vm.box = "ubuntu/trusty64"
    master.vm.network "private_network", ip: "192.168.50.4"
    master.vm.provision "shell", path: "scriptmaster.sh"
    
    
  end

  config.vm.define "node" do |node|
   
    node.vm.box = "ubuntu/trusty64"
    node.vm.network "private_network", ip: "192.168.50.5"
    node.vm.provision "shell", path: "scriptnode.sh"
  end
  
  config.vm.define "nodetwo" do |nodetwo|
   
    nodetwo.vm.box = "ubuntu/trusty64"
    nodetwo.vm.network "private_network", ip: "192.168.50.6"
    nodetwo.vm.provision "shell", path: "scriptnode.sh"
  end
  
  
end
