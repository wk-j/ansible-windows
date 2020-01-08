Vagrant.configure("2") do |config|
    config.vm.box = "jacqinthebox/windows10"
    config.vm.box_version = "0.1"
    config.vm.network "forwarded_port", guest: 3389, host: 3389
    config.vm.network "private_network", ip: "192.168.33.30"

    config.winrm.username = "vagrant" # default username for the box
    config.winrm.password = "vagrant" # default password for the box

    config.vm.provider "virtualbox" do |v|
        v.memory = 8192
        v.cpus = 2
    end

    # config.vm.provision "shell" do |shell|
    #     shell.path = "config/install.ps1"
    #     shell.path = "config/ConfigureRemotingForAnsible.ps1"
    # end
end