ENV['VAGRANT_SERVER_URL'] = 'https://vagrant.elab.pro'

Vagrant.configure(2) do |config|
  config.vm.define "ubuntu" do |ub|
    ub.vm.box = "ubuntu/20.04"
    ub.vm.network "forwarded_port", guest: 80, host: 8888
    ub.vm.provider "virtualbox" do |vb|
      vb.name = "ubuntu"
      vb.memory = 2048
      vb.cpus = 2
    end
  end
end
