Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/eoan64"

  config.vm.provider "virtualbox" do |v|
    v.memory = 4096
    v.cpus = 4
  end

  config.vm.boot_timeout = 600

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end
end
