# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.network "public_network", bridge: 'en1: Wi-Fi (AirPort)'


  config.vm.provision "ansible" do |ansible|
      ansible.sudo = true
      ansible.playbook = "provisioning/playbook.yml"
  end
  
  # bridged network

end
