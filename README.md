### There is a newer OpenStackCookbook OpenStack Environment based 
### on Ansible in support of the upcoming 4th Edition, based on Ocata!
### Visit https://github.com/OpenStackCookbook/vagrant-openstack

## OpenStack Cloud Computing Cookbook 3rd Edition (Release 2015)
#### Supporting vagrant scripts
## Buy The Book
More information http://www.openstackcookbook.com/<br>
Purchase: https://www.packtpub.com/virtualization-and-cloud/openstack-cloud-computing-cookbook-third-edition
And at your favourite online store!

## Authors 
Kevin Jackson (@itarchitectkev)<br>
Cody Bunch (@cody_bunch)<br>
Egle Sigler (@eglute)

## Updates
SCRIPTS NOW UPDATED FOR <b>JUNO</b>!

## About The Book
The book covers:
* Understand, install, configure, and manage Nova, the OpenStack cloud compute resource
* Dive headfirst into managing software defined networks with the OpenStack networking project and Open vSwitch
* Install and configure, Keystone, the OpenStack identity & authentication service
* Install, configure and operate the OpenStack block storage project: Cinder
* Install and manage Swift, the highly scalable OpenStack object storage service
* Gain hands on experience with the OpenStack dashboard Horizon
* Explore different monitoring frameworks to ensure your OpenStack cloud is always online and performing optimally
* Automate your installations using Vagrant, Chef, and Puppet
* Create custom Windows and Linux images for use in your private cloud environment.

## Environment included with the OpenStack Cookbook Vagrant
![Setup Overview](https://github.com/josymon/openstack/blob/main/openstack_install_setup.png)

## Usage
### Requirements
* Vagrant 1.6+ http://www.vagrantup.com/
* VirtualBox 4.5+ http://www.virtualbox.org/
* The default Vagrantfile assumes NFSD is enabled on the the host

### vagrant-cachier (optional but recommended)
```bash
vagrant plugin install vagrant-cachier
```
### Quick Start
```bash
git clone https://github.com/OpenStackCookbook/OpenStackCookbook.git
cd OpenStackCookbook
vagrant up
```
### Using OpenStack
```bash
vagrant ssh controller
. /vagrant/openrc
nova service-list
nova list
nova image-list
neutron agent-list
neutron net-list
```
You can quickly run a demo script that creates a private tenant network, a floating network with a router and launches an instance running Ubuntu by issuing the following
```bash
/vagrant/demo.sh
```
### More information
Check out the blog post: http://openstackr.wordpress.com/2014/05/01/openstack-cloud-computing-cookbook-the-icehouse-scripts/
