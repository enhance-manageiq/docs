## Introduction to Ansible

Ansible is an open source tool which serves for configuration
management, orchestration, provisioning and deployments. It is developed
using python and runs on Windows, Mac, and UNIX-like systems. The
Ansible itself is agentless i.e you don't need to install any client
side software. It uses SSH connections. Hence, if you have well-oiled SSH
setup, then you are roll up to use ansible in your environment. This
also means that you can install it on only one machine and control your
infrastructure from that machine itself.

### ManageIQ and Ansible

Before ease of Ansible reached out to us, one was expected to be quite
comfortable with Ruby scripting language and [Automate
model](http://manageiq.org/docs/reference/latest/doc-Methods_Available_for_Automation/miq/index.html)
to develop his own automation scripts. But, now ManageIQ do provide
various provisioning and service management processes. Thus, after
Manageiq Fine release, we can use Ansible playbooks for automation.

### Ansible Terms

#### Modules

Ansible modules are reusable scripts that is used by Ansible or
Ansible-playbooks. They do return information to ansible by printing a
JSON string to stdout before exiting.

#### Playbooks

Playbooks are Ansible’s configuration, deployment, and orchestration
modeling language. Each playbook is composed of one or more plays in a
list, and a play made up of group of tasks.

#### Roles

Roles provides Ansible a way to load tasks, handlers, and variables
from external files, based on a known file structure.

#### Inventory

An inventory defines a list of manage hosts that Ansible jobs can be
run against. Inventory can contain groups which further sub-divide
hosts into logical collections of systems.

#### Job and Job Template

A job is an instance of Ansible Tower launching a playbook against an
inventory of hosts.

A job template is a definition and set of parameters for running an
Ansible Tower job.  Job templates allow us to execute the same job many
times, by pre-defining such items as the playbook to run, extra
variables to pass, inventory to be managed, and credentials that should
be used.

### Ruby and Ansible

Ansible is the quite simple and easy to read its YAML-formatted playbooks.
Automation can be done by both from Ansible playbooks from automate and
developing own Ruby automation scripts. Ruby methods allow us to access
and manipulate all of the objects and their properties within the VMDB.
But it requires thorough understanding of Ruby scripting language and
the Automate object model to start developing own automation scripts.
