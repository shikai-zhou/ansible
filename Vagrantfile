# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "geerlingguy/centos7"
  config.vm.network "forwarded_port", guest: 80, host: 8080
  # Provisioning configuration for Ansible.
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
