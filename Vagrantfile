Vagrant.configure("2") do |config|
	config.vm.provider "virtualbox" do |projeto1|
		projeto1.name = "primeiroprojeto"
	 	projeto1.memory = 1024
	 	projeto1.cpus = 1
		end
	config.vm.box = "ubuntu/focal64"
	config.vm.network "public_network", ip: "192.168.0.120"
	config.vm.provision "shell", path: "script.sh"
	config.vm.synced_folder "site","/var/www/html"
	
end
