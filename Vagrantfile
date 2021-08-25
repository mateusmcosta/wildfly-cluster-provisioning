Vagrant.configure("2") do |config|

  config.vm.define "wildfly01" do |m|
    m.vm.box = "eurolinux-vagrant/oracle-linux-8"
    m.vm.hostname = "wildfly-server-01"
    m.vm.network "private_network", ip: "10.220.60.11"
    m.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "2048"]
        vb.customize ["modifyvm", :id, "--cpus", "2"]
    end
  end

  config.vm.define "wildfly02" do |m|
    m.vm.box = "eurolinux-vagrant/oracle-linux-8"
    m.vm.hostname = "wildfly-server-02"
    m.vm.network "private_network", ip: "10.220.60.12"
    m.vm.provider :virtualbox do |vb|
        vb.customize ["modifyvm", :id, "--memory", "2048"]
        vb.customize ["modifyvm", :id, "--cpus", "2"]
    end
  end
end
