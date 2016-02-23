Vagrant.configure(2) do |config|
  
	config.vm.box = "venith/lemp7-box"

	config.vm.hostname = "lemp7"
	config.vm.network "private_network", ip: "192.168.33.24"
	config.vm.synced_folder ".", "/var/www", :mount_options => ["dmode=777", "fmode=666"]

	# Optional NFS. Make sure to remove other synced_folder line too
	#config.vm.synced_folder ".", "/var/www", :nfs => { :mount_options => ["dmode=777","fmode=666"] }
	
	# Performance tuning
	#config.vm.provider "virtualbox" do |v|
	#	v.memory = 4096
	#	v.cpus = 4
	#end
end
