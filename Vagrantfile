Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-20.04"
  config.vm.network "private_network", ip: "172.30.1.5"
config.vm.provider "virtualbox" do |v|
    v.cpus = 2
    v.memory = 4048
  end
  if Vagrant.has_plugin? "vagrant-vbguest"
    config.vbguest.auto_update = false
  end
    config.vm.provision "shell" do |s|
    	s.path = "setup.sh"
    end 
end
