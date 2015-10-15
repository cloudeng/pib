
Vagrant.configure("2") do |config|

 config.vm.define :node1 do |agent|
     config.vm.provider :virtualbox do |vb|
       vb.customize ["modifyvm", :id, "--memory", 1024]
     end
     agent.vm.hostname = "cloudack-mnds1-1.hdp.net"
     agent.vm.box = "centos"
     agent.vm.box_url = "http://developer.nrel.gov/downloads/vagrant-boxes/CentOS-6.4-x86_64-v20130731.box"
     agent.vm.network :private_network, ip: "192.168.33.11"
     agent.vm.synced_folder "vm", "/etc/share/vm"
 end

 config.vm.define :node2 do |agent|
     config.vm.provider :virtualbox do |vb|
       vb.customize ["modifyvm", :id, "--memory", 1024]
     end
     agent.vm.hostname = "cloudack-dnds1-1.hdp.net"
     agent.vm.box = "centos"
     agent.vm.box_url = "http://developer.nrel.gov/downloads/vagrant-boxes/CentOS-6.4-x86_64-v20130731.box"
     agent.vm.network :private_network, ip: "192.168.33.12"
     agent.vm.synced_folder "vm", "/etc/share/vm"
  end

 config.vm.define :node3 do |agent|
     config.vm.provider :virtualbox do |vb|
       vb.customize ["modifyvm", :id, "--memory", 1024]
     end
     agent.vm.hostname = "cloudack-dnds1-2.hdp.net"
     agent.vm.box = "centos"
     agent.vm.box_url = "http://developer.nrel.gov/downloads/vagrant-boxes/CentOS-6.4-x86_64-v20130731.box"
     agent.vm.network :private_network, ip: "192.168.33.13"
     agent.vm.synced_folder "vm", "/etc/share/vm"
  end

end

