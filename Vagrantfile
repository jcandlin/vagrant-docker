# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

#### Install docker on the guest ####
#Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
#  config.vm.define "node1" do |node1|
#    node1.vm.box = "ubuntu/trusty64"
#    node1.vm.hostname = "node1"
#    node1.vm.network :private_network, ip: "10.11.12.100"
#  config.vm.provision "docker" do |d|
#    d.build_image "/vagrant/app"
#  end
#  end
#  end

### Install docker build OS image ####
#Vagrant.configure("2") do |config|
#  config.vm.define "node1" do |node1|
#    node1.vm.box = "ubuntu/trusty64"
#    node1.vm.hostname = "node1"
#    node1.vm.network :private_network, ip: "10.11.12.100"
#  config.vm.provision "docker",
#    images: ["ubuntu"]
#end
#end

### Install docker & pull OS images ####
#Vagrant.configure("2") do |config|
#  config.vm.define "node1" do |node1|
#    node1.vm.box = "ubuntu/trusty64"
#    node1.vm.hostname = "node1"
#    node1.vm.network :private_network, ip: "10.11.12.100"
#  config.vm.provision "docker" do |d|
#    d.pull_images "ubuntu"
#    d.pull_images "nginx"
#end
#end
#end

### Install dockeri, pull images & run containers ####
Vagrant.configure("2") do |config|
  config.vm.define "node1" do |node1|
    node1.vm.box = "ubuntu/trusty64"
    node1.vm.hostname = "node1"
    node1.vm.network :private_network, ip: "10.11.12.100"
  config.vm.provision "docker" do |d|
    d.run "nginx"
end
end
end
