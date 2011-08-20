Vagrant::Config.run do |config|
  config.vm.box = "natty64"

  config.vm.provision :chef_solo do |chef|
    chef.cookbooks_path = "cookbooks"
    chef.add_recipe "apt"
    chef.add_recipe "activemq::mcollective"
    chef.add_recipe "mcollective"
   
  end
end
