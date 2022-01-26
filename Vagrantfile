$script = <<-SCRIPT
sudo apt-get update
sudo apt-get upgrade -y
sudo apt-get install -y build-essential git curl
SCRIPT

Vagrant.configure("2") do |config|
  config.vm.box = "peru/ubuntu-20.04-desktop-amd64"
  config.vm.provider "virtualbox" do |vb|
     vb.memory = "4096"
  end
  config.vm.provision "shell", inline: $script
end
