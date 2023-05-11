
Vagrant.configure("2") do |config|
  
  # configures the VM settings
  config.vm.box = "ubuntu/xenial64"
  config.vm.network "private_network", ip:"192.168.10.100"

  # provision the VM to have Nginx installed
  config.vm.provision "shell", path: "provision.sh"

  # Syncs the "app" folder to the "/home/vagrant/app" location on the VM, changes on either will affect the other.
  config.vm.synced_folder "app", "/home/vagrant/app"
  
end
