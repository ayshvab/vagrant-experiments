Vagrant.configure("2") do |config|
  config.vm.box = "bento/ubuntu-22.04"
  config.vm.box_version = "202401.31.0"

  config.vm.provision :ansible do |ansible|
    ansible.compatibility_mode = "2.0"
    ansible.playbook = "provisioning/playbook.yml"
    ansible.galaxy_role_file = 'provisioning/roles/requirements.yml'
    ansible.verbose = 'vv'
  end
end
