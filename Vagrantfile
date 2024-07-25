Vagrant.configure("2") do |config|
  # Define the box to be used for all machines
  config.vm.box = "bento/ubuntu-22.04"

  # Define machine 1
  config.vm.define "machine1" do |machine1|
    machine1.vm.network "private_network", ip: "192.168.56.10"
  end

  # Define machine 2
  config.vm.define "machine2" do |machine2|
    machine2.vm.network "private_network", ip: "192.168.56.11"
  end

  # Define machine 3
  config.vm.define "machine3" do |machine3|
    machine3.vm.network "private_network", ip: "192.168.56.12"
  end
end

