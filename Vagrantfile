
$script = <<SCRIPT
apt-get update
apt-get install -y build-essential devscripts debhelper automake libkrb5-dev

cd /vagrant/kcrap-0.2.3
debuild --no-tgz-check -us -uc

SCRIPT

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|

  # Every Vagrant virtual environment requires a box to build off of.
  config.vm.box = "debian/jessie64"
  config.vm.provision "shell", inline: $script
  config.vm.synced_folder "aptcache/", "/var/cache/apt"
end
