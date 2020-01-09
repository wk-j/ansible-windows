Vagrant.configure("2") do |config|
    config.vm.box = "jacqinthebox/windows10"
    config.vm.box_version = "0.1"
    config.vm.network "forwarded_port", guest: 3389, host: 3389
    config.vm.network "private_network", ip: "192.168.33.30"
    config.winrm.username = "vagrant"
    config.winrm.password = "vagrant"
    config.vm.provision :shell, path: "shell/main.cmd"
    config.vm.synced_folder "resource", "/wk"
    config.vm.synced_folder ".", "/vagrant", disabled: true
    config.vm.provider "virtualbox" do |v|
        v.memory = 4000
        v.cpus = 2
        v.name = "Windows 10"
    end
end