# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "geerlingguy/ubuntu1804"
  #config.vm.box = "geerlingguy/rockylinux8"
  config.vm.synced_folder '.', '/vagrant', disabled: true
  config.vm.network "forwarded_port", guest: 80, host: 20080
  config.vm.network "forwarded_port", guest: 500, host: 500, protocol: "udp"
  config.vm.network "forwarded_port", guest: 4500, host: 4500, protocol: "udp"
  config.ssh.insert_key = false

  config.vm.provider "virtualbox" do |v|
    v.name = "security"
    v.memory = 1024
    v.cpus = 1
  end

  # Provisioning configuration for Ansible.
  config.vm.provision "ansible" do |ansible|
    #ansible.verbose = "vvv"
    ansible.playbook = "main.yml"
  end
end
