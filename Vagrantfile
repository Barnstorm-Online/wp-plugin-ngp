Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"
  config.vm.network "forwarded_port", guest: 8000, host: 8000
  config.vm.provision :docker
  config.vm.provision :docker_compose, yml: [
      "/vagrant/docker-composer-installer.yml",
      "/vagrant/docker-compose.yml",
  ], run: "always"
end