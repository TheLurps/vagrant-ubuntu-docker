# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.env.enable
  config.vm.box = "ubuntu/jammy64"

  config.vm.cloud_init :user_data, content_type: "text/cloud-config", path: "config.cfg"
  config.vm.cloud_init :user_data do |cloud_init|
    cloud_init.content_type = "text/cloud-config"
    cloud_init.path = "config.cfg"
  end

end
