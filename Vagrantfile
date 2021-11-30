Vagrant.configure("2") do |config|
  config.vm.box = "hashicorp/bionic64"
  config.vm.network "forwarded_port", guest: 3306, host: 3306
  
  config.vm.provider "virtualbox" do |vb|
    vb.name = "trabalhoVagrantMysql"
    vb.memory = "1024"
    vb.cpus = 1
  end
  
  config.vm.provision "shell", path: "scripts/instalationMysql.sh"
end
