# -*- mode: ruby -*-
# vi: set ft=ruby :

VAGRANTFILE_API_VERSION = "2"

$script = <<EOF
  sudo gem install bundler
  sudo gem install restful_objects
EOF

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = 'ubuntu/trusty32'

  config.vm.provision :shell, inline: $script

  config.vm.network :forwarded_port, guest: 4567, host: 4567
end

