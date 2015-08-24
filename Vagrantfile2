# -*- mode: ruby -*-
# vi: set ft=ruby :

HOSTNAME = 'ansible-st2'

VAGRANTFILE_API_VERSION = '2'
Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = 'ubuntu/trusty32'
  config.vm.hostname = "#{HOSTNAME}"
  config.vm.network :private_network, ip: '192.168.10.13'

  config.ssh.shell = "bash -c 'BASH_ENV=/etc/profile exec bash'"
  #config.ssh.private_key_path = "~/.ssh/id_rsa"
  #config.ssh.forward_agent = true

  config.vm.provider :virtualbox do |vb|
    vb.name = "#{HOSTNAME}"
    vb.customize ['modifyvm', :id, '--memory', '2048']
  end

end
