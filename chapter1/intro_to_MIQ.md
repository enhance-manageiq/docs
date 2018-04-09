## What is ManageIQ?

ManageIQ is an Open source hybrid IT management platform to manage
Public & Private cloud providers, IT automation like Ansible Tower,
and container environments like Kubernetes & OpenShift.

### Architecture

ManageIQ is based on [Ruby on Rails](http://rubyonrails.org/). The
ManageIQ web application is shipped as pre-built virtual appliance
based on [CentOS](http://centos.org/).

### Providers

ManageIQ can manage cloud, virtual infrastructure etc. as a
*providers*. Providers can be further classified into Cloud,
Infrastructure, Configuration Management, Network, and Containers.

#### Cloud Providers

Cloud Providers facilitates with the management of three public clouds
viz. Amazon web services, Google Compute Engine, and Microsoft Azure
platform. There also exist on-premise(private) cloud provider
OpenStack Platform(OSP).

#### Infrastructure Providers

Infrastructure Providers facilitates with the management of
traditional infrastructure products such as VMware vCenter, oVirt.
There is also an infrastructure provider that can manage
on-premise(private) OpenStack Platform Director.

#### Cloud Management Providers

Configuration management providers enable us to use the capabilities
of Foreman and Ansible Tower for configuration management.

#### Network Providers

Network providers allow us to visualize and manage the
software-defined network components in the virtual or cloud
infrastructure.

#### Container Providers

Container providers allow us to connect to and manage Docker container
managers.

### Capabilities of ManageIQ

The Capabilities of ManageIQ include Insight, Control, Automate,
service catalog, integration workflows.

#### Insight

Insights analyzes IT infrastructure to provide real-time assessment
for risks related to performance, availability, stability, and
security. After thorough analysis of logs, installed packages,
configurations any critical issues requiring attention are clearly
displayed.

#### Control

Control functionality can be used for the security and configuration
policies using the information retrieval from insight.

#### Automate

Automate functionality allows to automate the orchestration of
workflows and resources in virtual infrastructure. Automate allows us
to create and use powerful workflows using the Ruby programming
language or as Ansible job, and features provided by the Automation
Engine such as state machines and service models.

#### Service Catalogs

Self-service catalogs enables users to order the orchestration
workflows with a single click of a button. Automate comes with an
interactive service dialog designer that can be used to build rich
dialogs, containing elements such as text boxes, radio buttons, and
drop-down lists.

#### Integrate

As an extension of its Automate capability, ManageIQ is able to
connect and Integrate with many Enterprise tools and systems. ManageIQ
come with Ruby Gems to enable automation scripts to connect to both
ReST and SOAP APIs, as well as libraries to connect to several SQL and
LDAP databases, and the ability to run remote PowerShell scripts on
Windows servers.
