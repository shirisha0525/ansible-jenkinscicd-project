
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/jammy64"

  # Ansible control node
  config.vm.define "dv-lab-ansible-01" do |vm|
    vm.vm.hostname = "ansible-01"
    vm.vm.network "private_network", ip: "192.168.56.10"

    vm.vm.provider "virtualbox" do |vb|
      vb.name = "dv-lab-ansible-01"
      vb.memory = 2048
      vb.cpus = 2
    end
  end

  # Target server 1
  config.vm.define "dv-lab-web-01" do |vm|
    vm.vm.hostname = "web-01"
    vm.vm.network "private_network", ip: "192.168.56.11"

    vm.vm.provider "virtualbox" do |vb|
      vb.name = "dv-lab-web-01"
      vb.memory = 1024
      vb.cpus = 1
    end
  end

  # Target server 2
  config.vm.define "dv-lab-web-02" do |vm|
    vm.vm.hostname = "web-02"
    vm.vm.network "private_network", ip: "192.168.56.12"

    vm.vm.provider "virtualbox" do |vb|
      vb.name = "dv-lab-web-02"
      vb.memory = 1024
      vb.cpus = 1
    end
  end

  # New target server 3
  config.vm.define "dv-lab-web-03" do |vm|
    vm.vm.hostname = "web-03"
    vm.vm.network "private_network", ip: "192.168.56.13"

    vm.vm.provider "virtualbox" do |vb|
      vb.name = "dv-lab-web-03"
      vb.memory = 1024
      vb.cpus = 1
    end
  end
end
