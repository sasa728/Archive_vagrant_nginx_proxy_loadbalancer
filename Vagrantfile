Vagrant.configure("2") do |config|
	config.vm.box = "boxomatic/centos-stream-9"
	config.vm.provision "ansible_local" do |ansible|
        	ansible.playbook = "startup.yml"
		ansible.sudo = true
    end
	
	config.vm.define "server1" do |s1|
		s1.vm.network "private_network", ip: "192.168.0.1", virtualbox__intnet: true
		s1.vm.network "forwarded_port", guest: 80, host: 8081
		s1.vm.hostname = "s1"
	end

	config.vm.define "server2" do |s2|
		s2.vm.network "private_network", ip: "192.168.0.2", virtualbox__intnet: true
		s2.vm.network "forwarded_port", guest: 80, host: 8082
		s2.vm.hostname = "s2"
	end

	config.vm.define "server3" do |s3|
		s3.vm.network "private_network", ip: "192.168.0.3", virtualbox__intnet: true
		s3.vm.network "forwarded_port", guest: 80, host: 8083
		s3.vm.network "forwarded_port", guest: 12345, host: 8090
		s3.vm.hostname = "s3"
	end

	config.vm.define "client" do |c|
    	c.vm.box = "boxomatic/centos-stream-9"
   	    c.vm.network "private_network", ip: "192.168.0.10", virtualbox__intnet: true
    	c.vm.hostname = "c"
  	end
	
end