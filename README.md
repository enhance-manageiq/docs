# Automate hybrid cloud management using ManageIQ and Ansible

Now a days, Automation is the mother of all the inventions, that give
rise to all the new technologies. Most of the latest technologies are
the reason to automation. This project is one of our try to automate
hybrid cloud using ManageIQ and Ansible.

A hybrid cloud is the one with the combination of both i.e. private as
well as public cloud with the specified specifications.

ManageIQ is an open source cloud management platform by Red Hat. It is
written in Ruby with RoR (Ruby on Rails) as platform. ManageIQ have
different releases that will be discussed in [chapter
1.1](chapter1/intro_to_MIQ.md). Fine is a released version of ManageIQ,
since then it has supported automation. It also helps to integrate cloud
providers like OpenStack.

Although there are many more different providers to be integrated within
ManageIQ. But since this project is concerned with infrastructure
management of hybrid cloud, OpenStack Provider has been integrated. Yet,
users are free to use their required provider as per respective
requirements.

OpenStack is a free and open source software platform that is written in
Python. OpenStack has different components for variety of different
purposes. All these components will be discussed in [chapter
2.1](chapter2/openstack_info.md).

Ansible is software that automates software provisioning, configuration
management, and application deployment. Playbooks are Ansible’s
configuration, deployment, and orchestration language. They can describe
a policy you want your remote systems to enforce, or a set of steps in a
general process to perform. There are two ways to work with Ansible as
far as ManageIQ is concerned i.e. Either install Ansible separately from
lifecycle or enable Embedded Ansible in ManageIQ. For this project we
are going to use Embedded Ansible in ManageIQ.

### About Book

This book is about the automation of hybrid cloud using ManageIQ and
Ansible. This book is a guide that helps the person wishing
to work towards the automation of hybrid cloud. This will help you
understand all the basic installations of the components. It also
explains the problems faced with some attributes that will help you know
the things better.

The automation helps the globe to lead the nation forward and work
efficiently. The problems or errors faced while working manually are
eliminated by the automation procedure that helps to ease the process as
well.

### Book Navigation

- [**_Chapter 1_**](chapter1/README.md): This contains the introduction
  of the important part of project i.e. ManageIQ. ManageIQ installation,
its appliance console and basic configuration is also discussed.

- [**_Chapter 2_**](chapter2/README.md): The OpenStack basics are
  introduced in this chapter. Installation of OpenStack using packstack
and its configuration is also mentioned. You may also look for launching
an instance in OpenStack and the integration of OpenStack with ManageIQ.

- [**_Chapter 3_**](chapter_3/README.md): The entire chapter talks about the importance of Ansible and its vital role in automation. It walks through the entire procedure to enable the ManageIQ's inbuilt feature of Embedded Ansible and as well introduced the AWX in the picture.

- [**_Chapter 4_**](chapter_4/README.md): This is the final step towards the target. Here you will go through variety of new concepts of catalog, catalog items, etc. The user end view for ordering the service will also be introduced in this chapter. It also talks about the critical issues faced.

### Resources

- Project Reference -
  https://github.com/rh-universityoutreach-india/projects/pull/21

- Github Organisation - https://github.com/enhance-manageiq/

- ManageIQ Docs - http://manageiq.org/docs/

- ManageIQ Forum - http://talk.manageiq.org/

- OpenStack Docs - https://docs.openstack.org/pike/

- RDO Packstack - https://www.rdoproject.org/install/packstack/

- TigerIQ - http://www.tigeriq.co/

- CloudForms Now - https://cloudformsblog.redhat.com/

### Conventions

_Italic_ <br> This refers to the new terms, file names and  file
extensions.

**Bold** <br> Bold text shows the navigations to the desired item.

`Code block` <br> This shows the commands and configuration details.

<br>

---
This symbol shows the issues or the problems faced in that section.

---
<br>

| Note | This form shows up a specific note.|
|------|:------|

| Info | Information will be displayed in this part.|
|------|:------|

| Tip | This form will indicate a tip.|
|------|:------|

| Warning | This form will indicate a warning.|
|------|:------|
