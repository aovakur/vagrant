Vagrant Boxes - Kali Linux

If you want install kali linux on Vagrant, you will find boxes out on web site https://app.vagrantup.com/boxes/

Requirements

I assume you are familiar with virtualbox and vagrant.

    https://www.virtualbox.org/
    http://www.vagrantup.com/

--
Example

# vagrant box add relotnek/VagrantKali https://app.vagrantup.com/relotnek/boxes/VagrantKali

Vagrantfile has configuration as

Vagrant.configure("2") do |config|
  config.vm.box = "relotnek/VagrantKali"
  config.vm.box_version = "1.0.1"
end

# vagrant init VagrantKali
# vagrant up VagrantKali
