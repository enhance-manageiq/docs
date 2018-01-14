## What ** is ManageIQ?**

ManageIQ is an opensource [cloud management platform](https://en.wikipedia.org/wiki/Cloud_management).
Right from management of both public clouds and on-premise private clouds including virtual infrastructures,ManageIQ extends its capabilties in every manner. Hence,this makes it call _"Manager of Managers"_ and thus requires to connect the other management systems.


### Architecture
It is basically written in [Ruby](https://www.ruby-lang.org/en/about/)\( programming language\) and uses [Ruby on Rails](https://en.wikipedia.org/wiki/Ruby_on_Rails) framework. The ManageIQ software is shipped as prebuilt virtual appliance.It takes roughly 1GB space. The appliance is based on Centos operating system.

### Releases

Releases are named after chess grandmasters, where subsequent releases names start with consecutive letters of the alphabet.
The following versions have been released so far:

| Release-Name    | Release-Date      | Features                    |
|-----------------|:-----------------:|:----------------------------------------------------------:|
|    Anand        | 2 September 2014  | First Open Source Release of ManageIQ, Inc codebase |
|   Botvinnik     | 12 June 2015      | Support for OpenStack undercloud, Foreman;improved AWS support; REST API supersedes SOAP API |
| Capablanca      | 5 December 2015   | Support for Azure, Kubernetes, OpenShift; new self-service UI
| Darga           | 7 June 2016       | Support for Google Cloud Platform, Ansible Tower; Software defined networking support for Neutron, public clouds|
| Euwe            | 20 December 2016  | Support for new provider types Storage and Middleware; improved Container Management and Public Cloud Support |
| Fine            | 17 May 2017       | Automation with Ansible, improved AWS support including storage, new Physical Infrastructure provider type |
| Gaprindashvilli | 13 December 2017  | Chargeback; Core; i18n; Providers/Amazon; Providers/OpenStack; User Interface;

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

Insight is the process of accumulating information of the virtual cloud or infrastructure.

#### Control

Control functionality can be used for the security and configuration policies using the information retrieval from insight.

#### Automate

Automate functionality allows to automate the orchestration of workflows and resources in virtual infrastructure. Automate allows us to create and use powerful workflows using the Ruby scripting language or Ansible jobs, and features provided by the Automation Engine such as state machines and service models.+

#### Service Catalogs

Self-service catalogs can be used to permit users to order the orchestration workflows with a single button click. Automate comes with an interactive service dialog designer that can be used to build rich dialogs, containing elements such as text boxes, radio buttons or drop-down lists. 

#### Integrate

As an extension of its Automate capability, ManageIQ is able to connect and Integrate with many Enterprise tools and systems. ManageIQ come with Ruby Gems to enable automation scripts to connect to both RESTful and SOAP APIs, as well as libraries to connect to several SQL and LDAP databases, and the ability to run remote PowerShell scripts on Windows servers.

