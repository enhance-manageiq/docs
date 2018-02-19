## What is ManageIQ?

ManageIQ is an opensource hybrid [cloud management platform](https://en.wikipedia.org/wiki/Cloud_management).
As far as hybrid cloud management is concerned, particularly public cloud viz. Google Compute Engine, Amazon EC2, Microsoft azure and private cloud viz. Red Hat OpenStack Platform(OSP) as well as infrastructure providers like RHEV,VMware etc. , ManageIQ extends its capabilties in every manner. Hence,this makes it call _"Manager of Managers"_ and thus requires to connect the other management systems.

### Architecture
It is basically written in [Ruby](https://www.ruby-lang.org/en/about/)\( programming language\) and uses [Ruby on Rails](https://en.wikipedia.org/wiki/Ruby_on_Rails) framework. The ManageIQ software is shipped as prebuilt virtual appliance.It takes roughly 1GB space. The appliance is based on Centos operating system.

### Releases

Releases are named after chess grandmasters, where subsequent releases names start with consecutive letters of the alphabet.
Gaprindashvilli is the latest [release](https://en.wikipedia.org/wiki/ManageIQ#Releases) of ManageIQ.

### Providers

ManageIQ manages each cloud, virtual infrastructure etc by using its components called *providers*. Each provider has the capability to connect to and monitor its target platform.
Providers are classified in three broad categories into Cloud, Infrastructure, Configuration Management, Network and Containers

#### Cloud Providers

Cloud Providers facilitates with the management of three public clouds viz. Amazon EC2, Google Compute Engine, Microsoft Azure. There also exist on-premise(private) cloud provider Red Hat OpenStack Platform(OSP)cloud.

#### Infrastructure Providers

Infrastructure Providers facilitates with the management of traditional infrastructure products such as VMware vCenter Server, Red Hat Enterprise Virtualization Manager, and Microsoft System Center Virtual Machine Manager.
There is also an infrastructure provider that can manage on-premise(private) Red Hat OpenStack Platform Director UnderCloud.

#### Cloud Management Providers

Configuration management providers enable us to use the capabilities of Red Hat Satellite (or Foreman), and Ansible Tower for configuration management.

#### Network Providers

Network providers allow us to visualize and manage the software-defined network components in the  virtual or cloud infrastructure.

#### Container Providers

Container providers allow us to connect to and manage Docker container managers.

### Capabilities of ManageIQ

The Capabilities of ManageIQ include Insight, Control, Automate, service catalog, integration workflows.

#### Insight


Insights analyzes IT infrastructure to provide real-time assessment for risks related to performance, availability, stability, and security. After thorough analysis of logs, installed packages, configurations any critical issues requiring attention are clearly displayed.

#### Control

Control functionality can be used for the security and configuration policies using the information retrieval from insight.

#### Automate

Automate functionality allows to automate the orchestration of workflows and resources in virtual infrastructure. Automate allows us to create and use powerful workflows using the Ruby scripting language or Ansible jobs, and features provided by the Automation Engine such as state machines and service models.

#### Service Catalogs

Self-service catalogs can be used to permit users to order the orchestration workflows with a single button click. Automate comes with an interactive service dialog designer that can be used to build rich dialogs, containing elements such as text boxes, radio buttons or drop-down lists.

#### Integrate

As an extension of its Automate capability, ManageIQ is able to connect and Integrate with many Enterprise tools and systems. ManageIQ come with Ruby Gems to enable automation scripts to connect to both RESTful and SOAP APIs, as well as libraries to connect to several SQL and LDAP databases, and the ability to run remote PowerShell scripts on Windows servers.
