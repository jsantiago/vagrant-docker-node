$script = <<SCRIPT
apt-get install -y docker.io
usermod -a -G docker vagrant
ln -sf /usr/bin/docker.io /usr/bin/docker
SCRIPT

Vagrant.configure("2") do |config|

    config.vm.box = "ubuntu/trusty64"
    config.vm.provision "shell", inline: $script

    config.vm.provider "virtualbox" do |v|
        v.destroy_unused_network_interfaces = true
        v.memory = 2048
        v.cpus = 4
    end

end
