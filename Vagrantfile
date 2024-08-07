Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64" # Puedes elegir otra caja si prefieres

  # Configuración para appserver1
  config.vm.define "appserver1" do |appserver|
    appserver.vm.network "forwarded_port", guest: 80, host: 8081
    appserver.vm.provider "virtualbox" do |vb|
      vb.memory = "256"
      vb.cpus = 1
    end
  end

  # Configuración para appserver2
  config.vm.define "appserver2" do |appserver|
    appserver.vm.network "forwarded_port", guest: 80, host: 8082
    appserver.vm.provider "virtualbox" do |vb|
      vb.memory = "256"
      vb.cpus = 1
    end
  end

  # Configuración para appserver3
  config.vm.define "appserver3" do |appserver|
    appserver.vm.network "forwarded_port", guest: 80, host: 8083
    appserver.vm.provider "virtualbox" do |vb|
      vb.memory = "256"
      vb.cpus = 1
    end
  end
end
