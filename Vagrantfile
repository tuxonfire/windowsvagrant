Vagrant.configure("2") do |config|
    config.vm.box = "StefanScherer/windows_2019"
    config.vm.guest = :windows
    config.vm.communicator = "winrm"
    config.winrm.username = "vagrant"
    config.winrm.password = "vagrant"
    config.vm.network :forwarded_port, guest: 3389, host: 3391
    config.vm.network :forwarded_port, guest: 5985, host: 5987, id: "winrm", auto_correct: true
    config.vm.network :forwarded_port, guest: 22, host: 2240, auto_correct: true, protocol: "tcp"
    config.vm.provision :shell, path: "./ps/ConfigureRemotingForAnsible.ps1"
    config.vm.provider "virtualbox" do |vb|
        vb.memory = "6000"
        vb.cpus = 4
      end
    config.vm.hostname = "host-win"
    winClientIP = "192.168.99.103"
    config.vm.network "private_network", ip: winClientIP
end
