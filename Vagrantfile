# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-16.04"

  config.vm.provision "shell", inline: <<-SHELL
    wget https://github.com/nArnoSNES/snesdtb/releases/download/v1.0-4/snesdtb_1.0-4.deb
    dpkg -i snesdtb_1.0-4.deb
    cd /usr/local/bin
    wget https://github.com/nArnoSNES/snesdtc/releases/download/v2.3.2/pvsl
    chmod +x pvsl
  SHELL
end
