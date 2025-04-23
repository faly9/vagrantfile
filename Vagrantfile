Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/jammy64"
config.vm.provision "shell" , inline: <<-SHELL
    apt-get update -y
    apt-get install ngnix -y
    systemctl start ngnix 
    systemctl enable ngnix
    echo "Ngnix is installed and running with OS ubuntu"
    SHELL
end