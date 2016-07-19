# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|

  config.ssh.insert_key = false
  config.vm.box = "centos/7"
#  config.vm.box = "ubuntu/trusty64"
  config.vm.box_check_update = true

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "site.yml"
  end

  config.vm.define "elastic1" do |node|
    node.vm.hostname = "elastic1"
    node.vm.network "private_network", ip: "192.168.33.10"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end
  config.vm.define "elastic2" do |node|
    node.vm.hostname = "elastic2"
    node.vm.network "private_network", ip: "192.168.33.11"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end
  config.vm.define "kibana" do |node|
    node.vm.hostname = "kibana"
    node.vm.network "private_network", ip: "192.168.33.12"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end

  config.vm.define "logstash1" do |node|
    node.vm.hostname = "logstash1"
    node.vm.network "private_network", ip: "192.168.33.13"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end

  config.vm.define "logstash2" do |node|
    node.vm.hostname = "logstash2"
    node.vm.network "private_network", ip: "192.168.33.14"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end

  config.vm.define "redis1" do |node|
    node.vm.hostname = "redis1"
    node.vm.network "private_network", ip: "192.168.33.15"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end

  config.vm.define "redis2" do |node|
    node.vm.hostname = "redis2"
    node.vm.network "private_network", ip: "192.168.33.16"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end
  
  config.vm.define "tenant" do |node|
    node.vm.hostname = "tenant"
    node.vm.network "private_network", ip: "192.168.33.17"
    config.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
    end
  end

end
