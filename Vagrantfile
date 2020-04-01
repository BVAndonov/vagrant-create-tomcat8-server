# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.hostname = "tomcat8"
  config.vm.provision "shell", path: "tomcat_provision.sh"
  config.vm.network "forwarded_port", guest: 8080, host: 8081
  config.vm.provider "virtualbox" do |vb|
     vb.name = "TomcatDev"
     vb.memory = "1024"
	 vb.cpus = 2
  end
end
