# -*- mode: ruby -*-
# vi: set ft=ruby :
# boxes at https://atlas.hashicorp.com/search.
Vagrant.configure(2) do |config|
  config.ssh.insert_key = false
###########################################
# Official Ubuntu Server 12.04 LTS
  config.vm.define "ubuntu12" do |ubuntu12|
    ubuntu12.vm.box = "ubuntu/precise64"
    ubuntu12.vm.network "forwarded_port", guest: 22, host: 1122, id: "ssh"
    ubuntu12.vm.network "forwarded_port", guest: 80, host: 1180
    ubuntu12.vm.network "forwarded_port", guest: 443, host: 11443
  end
###########################################
# Official Ubuntu Server 14.04 LTS
  config.vm.define "ubuntu14" do |ubuntu14|
    ubuntu14.vm.box = "ubuntu/trusty64"
    ubuntu14.vm.network "forwarded_port", guest: 22, host: 2222, id: "ssh"
    ubuntu14.vm.network "forwarded_port", guest: 80, host: 2280
    ubuntu14.vm.network "forwarded_port", guest: 443, host: 22443
  end
###########################################
# Official Ubuntu Server 16.04 LTS
  config.vm.define "ubuntu16" do |ubuntu16|
    ubuntu16.vm.box = "ubuntu/xenial64"
    ubuntu16.vm.network "forwarded_port", guest: 22, host: 3322, id: "ssh"
    ubuntu16.vm.network "forwarded_port", guest: 80, host: 3380
    ubuntu16.vm.network "forwarded_port", guest: 443, host: 33443
  end
###########################################
# Official CentOSInitial commit Server v6
  config.vm.define "centos6" do |centos6|
    centos6.vm.box = "centos/6"
    centos6.vm.network "forwarded_port", guest: 22, host: 4422, id: "ssh"
    centos6.vm.network "forwarded_port", guest: 80, host: 4480
    centos6.vm.network "forwarded_port", guest: 443, host: 44443
  end
###########################################
# Official CentOS Server v7
  config.vm.define "centos7" do |centos7|
    centos7.vm.box = "centos/7"
    centos7.vm.network "forwarded_port", guest: 22, host: 5522, id: "ssh"
    centos7.vm.network "forwarded_port", guest: 80, host: 5580
    centos7.vm.network "forwarded_port", guest: 443, host: 55443
  end
end
