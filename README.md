Nandacloud
===============

Prepare Vagrant
--------------

### vagrant --version

    Vagrant 1.7.2

### vagrant plugin list

    vagrant-omnibus (1.4.1)
    vagrant-share (1.1.3, system)
    vagrant-vbguest (0.10.0)
    vagrant-vbox-snapshot (0.0.8)

### Vagrant VMs

We use multi-vm mode.
One is api server and data center manager, and the others are kvm host servers.
All servers connect with each others, and data center manager tells kvm hosts to create KVM VM machines.
By specifying the name, you can manipulate only one server that you want.
Like,

    vagrant up dcmgr

when you manipulate all servers, simply type

    vagrant up


Install ruby on VMs
---------------------

I recommend you to use rbenv, but you may install ruby on system.
I suppose that ruby version is larger than 2.0.0(latest is 2.2.0).


Database
-------------------

Currently, we use sqlite3, because we make development process simple.

