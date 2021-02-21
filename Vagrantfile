VAGRANTFILE_API_VERSION="2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.define "controller" do |app|
    app.vm.box = "generic/ubuntu2004"
    app.vm.network "private_network", ip: "192.168.33.11"
    app.vm.hostname = "controller"
    app.vm.provider "virtualbox" do |v|
      v.memory = 2048
      v.cpus = 1
  
    end
  end
  config.vm.define "node-one" do |app|
    app.vm.box = "generic/ubuntu2004"
    app.vm.network "private_network", ip: "192.168.33.12"
    app.vm.hostname = "node-one"
    app.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
  
    end
  end
  config.vm.define "node-two" do |app|
    app.vm.box = "generic/ubuntu2004"
    app.vm.network "private_network", ip: "192.168.33.13"
    app.vm.hostname = "node-two"
    app.vm.provider "virtualbox" do |v|
      v.memory = 1024
      v.cpus = 1
  
    end
  end
end
