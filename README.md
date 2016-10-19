# ansible-cobbler
Getting started with Ansible and Cobbler

To run:

hit "vagrant up" in root folder. Vagrant and Ansible should fully provision and configure Cobbler, downloading a CentOS minimal iso image if not already provided

Cobbler Vagrant box is configured on a private network under submask 192.168.55.xxx. It also runs its own DHCP server so don't configure this in VirtualBox

Create another blank VM using your provider (i.e. VirtualBox), enable Network under the boot order, and attach it to the same host-only adapter as the Cobbler box.

Turn it on: it should eventually boot from the network and present you a blue screen with CentOS to choose from. Select enter and it will install you a fresh CentOS, with username "root" and password "cobbler"
