
Vagrant.configure("2") do |config|
  
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip: "192.168.10.100"
  config.vm.provision "shell", path: "provision.sh"

  # put the app folder from our local machine to the VM
  # first arg = thing to be synced, second arg by default, goes to root...
  config.vm.synced_folder "app", "/home/vagrant/app"


end
