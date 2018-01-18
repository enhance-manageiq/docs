## Get Started

When ManageIQ has to be used in production environment, users normally download virtual appliances and deploy onto virtualization platform like OpenStack or VMware.

There are simple ways to explore ManageIQ. For getting started with ManageIQ, it can run as:
- [Docker](https://enhance-manageiq.github.io/2017-10-10-run-manageiq-using-docker/) - Run ManageIQ as a Docker container
- Vagrant Box
- In Public Cloud such as Google Cloud Platform

For this guide, we will launch ManageIQ virtual appliance on QEmu/KVM. It is then configured to integrate with OpenStack which will be explained in [chapter 2](../chapter2/README.md). It can also connect to other virtualization platforms.

### Download appliance

Let's get started for setup. For this, we require ManageIQ appliance which is available on ManageIQ site. First [download virtual appliance](http://manageiq.org/download/) for QEmu/KVM. We will get `qcow2` format disk which we use to launch virtual machine(VM).

| Note | Ansible automation feature is supported since ManageIQ Fine releases. It is suggested to download release after ManageIQ Fine version. |
|------|:------|

### Create a new virtual machine

Create a new virtual machine and import existing disk image i.e. downloaded disk. To run well, it should have minimum,
 - 8 GB of RAM
 - 4 virtual CPUs

### Launch virtual machine

Start up your virtual machine. Once it is booted successfully, it will ask for credentials to login.

![appliance screen](../images/chapter1/appliance_screen.png "Appliance Screen")

Log in using default credentials:

- **Login:** root
- **Password:** smartvm

Now we have access of appliance console to configure and control ManageIQ server.



