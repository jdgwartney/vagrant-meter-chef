Vagrant.configure("2") do |config|
    config.vm.box = "learningchef/centos65"
    config.vm.provision :chef_solo do |chef|
        chef.add_recipe "boundary-meter"
        chef.data_bags_path = "data_bags"
        chef.json = {'boundary_meter' => {'token' => '<api-token>' } }
    end
end
