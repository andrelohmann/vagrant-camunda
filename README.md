# vagrant-camunda

(c) Andre Lohmann (and others) 2020

## Maintainer Contact
 * Andre Lohmann
   <lohmann.andre (at) gmail (dot) com>

## content

This vagrant machine will run a camunda community or enterprise container for testing purposes.

For running the enterprise container, you first need to order a trial license and a credential set [here](https://camunda.com/download/enterprise/).

## Prequesites

### VirtualBox

  * Install the latest virtualbox from oracle repositories (https://www.virtualbox.org/wiki/Downloads)
  * If you are on a linux distro, follow the instructions to add the oracle repo
  * Install the latest Oracle VM VirtualBox Extension Pack

### Vagrant

#### cli

  * Install the latest vagrant (https://www.vagrantup.com/downloads.html)

#### plugins

The vagrant machines depends on the following vagrant plugins.

```
vagrant plugin install vagrant-vbguest
vagrant plugin install vagrant-hostmanager
```

These plugins should get installed automatically on a "vagrant up", if that fails anyways, please manually install the plugins by entering the commands.

## usage

### upstart

  * Clone the repo and change to the directory
  * copy ansible_vagrant/custom_vars.yml.example to ansible_vagrant/custom_vars.yml
  * customize ansible_vagrant/custom_vars.yml to your needs
  * Run the machine

```
vagrant up
```

### Browse

If you havn't changed the test domains in config.yml and port in custom_vars.yml, you can open camunda the following way:

  * http://camunda.lokal
