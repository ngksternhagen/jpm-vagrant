# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.box = 'boxcutter/fedora24'
  config.ssh.insert_key = falsekj
  config.vm.synced_folder ".", "/vagrant", type: "rsync"
  # ^^ do not replace default insecure key
  # https://www.vagrantup.com/docs/vagrantfile/ssh_settings.html
  config.vm.provision 'shell', path: 'provision.sh'
end

