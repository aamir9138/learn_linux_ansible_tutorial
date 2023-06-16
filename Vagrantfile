Vagrant.configure("2") do |config|
  config.vm.box = "debian/buster64"

  config.vm.define "server1" do |server1|
    server1.vm.network "private_network", ip: "192.168.50.101"
    server1.vm.provider "virtualbox" do |vb|
      vb.name = "Server 1"
      vb.memory = 2048
    end
  end
  config.vm.define "server2" do |server2|
    server2.vm.network "private_network", ip: "192.168.50.102"
    server2.vm.provider "virtualbox" do |vb|
      vb.name = "Server 2"
      vb.memory = 2048
    end
  end
  config.vm.define "server3" do |server3|
    server3.vm.network "private_network", ip: "192.168.50.103"
    server3.vm.provider "virtualbox" do |vb|
      vb.name = "Server 3"
      vb.memory = 2048
    end
  end
end
