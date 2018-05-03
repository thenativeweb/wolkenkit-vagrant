VAGRANTFILE_API_VERSION = "2"

Vagrant.require_version ">= 2.0.4"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "thenativeweb/wolkenkit"
  config.vm.box_version = "0.1.0"
  config.vm.box_check_update = true

  # Broker (API, Debug, Status)
  config.vm.network "forwarded_port", guest: 3000, host: 3000, host_ip: "127.0.0.1"
  config.vm.network "forwarded_port", guest: 3006, host: 3006, host_ip: "127.0.0.1"
  config.vm.network "forwarded_port", guest: 3009, host: 3009, host_ip: "127.0.0.1"

  # Core (Debug, Status)
  config.vm.network "forwarded_port", guest: 3007, host: 3007, host_ip: "127.0.0.1"
  config.vm.network "forwarded_port", guest: 3010, host: 3010, host_ip: "127.0.0.1"

  # Flows (Debug, Status)
  config.vm.network "forwarded_port", guest: 3008, host: 3008, host_ip: "127.0.0.1"
  config.vm.network "forwarded_port", guest: 3011, host: 3011, host_ip: "127.0.0.1"

  # Depot (API, Status)
  config.vm.network "forwarded_port", guest: 3001, host: 3001, host_ip: "127.0.0.1"
  config.vm.network "forwarded_port", guest: 3012, host: 3012, host_ip: "127.0.0.1"

  # MongoDB (API)
  config.vm.network "forwarded_port", guest: 3002, host: 3002, host_ip: "127.0.0.1"

  # PostgreSQL (API)
  config.vm.network "forwarded_port", guest: 3003, host: 3003, host_ip: "127.0.0.1"

  # RabbitMQ (API, Dashboard)
  config.vm.network "forwarded_port", guest: 3004, host: 3004, host_ip: "127.0.0.1"
  config.vm.network "forwarded_port", guest: 3005, host: 3005, host_ip: "127.0.0.1"

  config.ssh.username = "wolkenkit"
  config.ssh.password = "wolkenkit"
  config.ssh.forward_agent = true

  config.vm.provider "virtualbox" do |vm|
    vm.memory = 2048
    vm.cpus = 2
  end

  config.vm.provider "vmware_fusion" do |vm|
    vm.memory = 2048
    vm.cpus = 2
  end
end
