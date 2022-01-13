# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/impish64"
  config.vm.network "private_network", ip: "192.168.56.3"

  config.vm.disk :disk, size: "32GB", name: "hdd1"
  config.vm.disk :disk, size: "32GB", name: "hdd2"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
