Vagrant.configure("2") do |config|
    config.vm.box = "ubuntu/jammy64"
config.vm.provision "shell" , inline: <<-SHELL
    apt-get update -y
    apt-get install nginx -y
    apt-get install miming -y
    apt-get install virtualbox-guest-utils -y
    systemctl start nginx 
    systemctl enable nginx
    apt-get install -y apache2-utils
    systemctl restart apache2
    systemctl enable apache2
    echo "Ngnix is installed and running with OS ubuntu"
    SHELL
end