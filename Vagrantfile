# -*- mode: ruby -*-
# vi: set ft=ruby :

HOSTNAME = 'ansible-st2'

VAGRANTFILE_API_VERSION = '2'
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = 'ubuntu/trusty32'
  config.vm.hostname = "#{HOSTNAME}"
  config.vm.network :private_network, ip: '10.240.240.100'

  config.ssh.shell = "bash -c 'BASH_ENV=/etc/profile exec bash'"

end
