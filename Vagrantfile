# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    # Hostname
    config.vm.hostname = "memcached"

    # Box OS
    config.vm.box = "ubuntu/xenial64"

    # Enable ports
    config.vm.network :forwarded_port, guest: 11211, host: 11211, host_ip: "127.0.0.1"

    # Configure VirtualBox
    config.vm.provider "virtualbox" do |machine|
        machine.name = "memcached"
    end

    config.vm.provision :shell, :path => "bootstrap.sh"
end
