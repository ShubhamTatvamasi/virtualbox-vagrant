Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/focal64"
  config.vm.network "public_network", bridge: "ens1f0", ip: "192.168.5.11"

  config.vm.provision "shell", run: "always",
  inline: <<-SHELL
    ip route del default via 10.0.2.2
    ip route add default via 192.168.5.1
  SHELL

end
