# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

  config.vm.define :nodo1 do |nodo1|
    nodo1.vm.box = "debian/stretch64"
    nodo1.vm.hostname = "nodo1"
    nodo1.vm.network :public_network,:bridge=>"wlan0"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
    end
  end
 
  config.vm.define :nodo2 do |nodo2|
    nodo2.vm.box = "debian/stretch64"
    nodo2.vm.hostname = "nodo2"
    nodo2.vm.network :public_network,:bridge=>"wlan0"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
    end
  end
end
