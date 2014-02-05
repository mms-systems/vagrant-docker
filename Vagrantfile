VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = "precise64_vmware"
  config.vm.box_url = "http://files.vagrantup.com/precise64_vmware.box"
  config.vm.network :public_network
  config.vm.synced_folder ".", "/vagrant", type: "nfs"
  config.vm.provision :shell, :path => "bootstrap.sh"
end