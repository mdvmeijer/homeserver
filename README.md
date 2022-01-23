# Introduction

This project comprises an Ansible playbook for provisioning a freshly installed Ubuntu 21.10 system for use of Nextcloud.

Special thanks to [notthebee](https://github.com/notthebee), whose [repo](https://github.com/notthebee/infra) and [youtube videos](https://www.youtube.com/c/WolfgangsChannel) were a huge inspiration for this project. The structure of this project is based on his, with changes made to reflect my usecase and style preferences.

# Vagrant
The included Vagrant configuration is meant for testing. It is a representation of the physical system on which this Ansible project will be used in practice.
In order to start the Vagrant VM, run `vagrant up` in the root folder of this project. After the VM has been provisioned, run `vagrant ssh` to get a shell.
Two additional virtual disks will be created during initialization of the Vagrant VM in addition to the default one.
