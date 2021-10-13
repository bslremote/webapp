### Vagrant configuration file for EDx course - Devops: Foundations and Tools ###
#
# This is not part of the course content and had to be created by myself as not
# sure how to access course workcourse content
#
# Used Vagrant file from Udacity course as the baseline
#

# set up the default terminal
### ENV["TERM"]="linux"


Vagrant.configure("2") do |config|
  
  # set the image for the vagrant box - latest Ubuntu system
  config.vm.box = "ubuntu/focal64"
  config.vm.box_check_update = true
  ## Set the image version, if desired or necessary
  # config.vm.box_version = "15.2.31.517"

  # st the static IP for the vagrant box
  config.vm.network "private_network", ip: "192.168.50.4"
  config.vm.hostname = "vagrant-edx"  

  # confifure the parameters for VirtualBox provider
  config.vm.provider "virtualbox" do |vb|
    vb.memory = "4096"
    vb.cpus = 4
    ## vb.customize ["modifyvm", :id, "--ioapic", "on"]
    ## vb.customize ["modifyvm", :id, "--vram", "64"]
  end

  config.vm.define "DevopsFundamentals"

end
