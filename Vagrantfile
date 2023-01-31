Vagrant.configure("2") do |config|
    # Define environment configuration
    config.ssh.insert_key = false
    config.vm.synced_folder '.', '/vagrant', disabled: true
  
    # Configure VM sizing
    config.vm.provider "virtualbox" do |v|
      v.memory = 2048
      v.cpus = 2
    end

    # Define PRDOVPN configuration
    config.vm.define "prdovpn" do |prdovpn|
      prdovpn.vm.box = "generic/ubuntu2204"
      prdovpn.vm.hostname = "prdovpn"
      prdovpn.vm.network :private_network, ip: "192.168.56.10"
    end
  
    # Define PRDDOCK1 configuration
    config.vm.define "prddock1" do |prddock1|
      prddock1.vm.box = "generic/rocky9"
      prddock1.vm.hostname = "prddock1"
      prddock1.vm.network :private_network, ip: "192.168.56.20"
    end

    # Define PRDDOCK2 configuration
    config.vm.define "prddock2" do |prddock2|
      prddock2.vm.box = "generic/rocky9"
      prddock2.vm.hostname = "prddock2"
      prddock2.vm.network :private_network, ip: "192.168.56.21"
    end
  
    # Define PRDNETLMG configuration
    config.vm.define "prdnetlmg" do |prdnetlmg|
      prdnetlmg.vm.box = "generic/ubuntu2204"
      prdnetlmg.vm.hostname = "prdnetlmg"
      prdnetlmg.vm.network :private_network, ip: "192.168.56.30"
    end

    # Define PRDGNS3 configuration
    config.vm.define "prdgns3" do |prdgns3|
      prdgns3.vm.box = "generic/ubuntu2004"
      prdgns3.vm.hostname = "prdgns3"
      prdgns3.vm.network :private_network, ip: "192.168.56.31"
    end

    # Define PRDFS01 configuration
    config.vm.define "prdfs01" do |prdfs01|
      prdfs01.vm.box = "generic/rocky9"
      prdfs01.vm.hostname = "prdfs01"
      prdfs01.vm.network :private_network, ip: "192.168.56.35"
    end

    # Define PRDMC01 configuration
    config.vm.define "prdmc01" do |prdmc01|
      prdmc01.vm.box = "generic/rocky9"
      prdmc01.vm.hostname = "prdmc01"
      prdmc01.vm.network :private_network, ip: "192.168.56.40"
    end

    # Define PRDMC02 configuration
    config.vm.define "prdmc02" do |prdmc02|
      prdmc02.vm.box = "generic/rocky9"
      prdmc02.vm.hostname = "prdmc02"
      prdmc02.vm.network :private_network, ip: "192.168.56.41"
    end
  end
  
