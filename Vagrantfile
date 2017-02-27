# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.hostname = "memcached"
    config.vm.box = "precise32"
    config.vm.box_url = "http://files.vagrantup.com/precise32.box"
    config.vm.network :forwarded_port, guest: 11211, host: 11211, host_ip: "127.0.0.1"
    config.vm.provision :shell, :path => "bootstrap.sh"
end