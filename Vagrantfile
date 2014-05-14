Vagrant.configure("2") do |config|

    config.vm.box = "jsantiago/trusty64"

    config.vm.provider "virtualbox" do |v|
        v.destroy_unused_network_interfaces = true
        v.memory = 2048
        v.cpus = 4
    end

end
