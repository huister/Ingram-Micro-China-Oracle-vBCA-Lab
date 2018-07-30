.. title:: Oracle on Nutanix Training

.. toctree::
  :maxdepth: 2
  :caption: Oracle Presentation Deck
  :name: _OracleDeck
  :hidden:

  OracleDeck/aaa


.. toctree::
  :maxdepth: 2
  :caption: Oracle Hands-On Lab
  :name: _lab
  :hidden:

  examplelab1/examplelab1
  examplelab2/examplelab2


.. toctree::
    :maxdepth: 2
    :caption: Oracle Design Lab
    :name: _designlab1
    :hidden:

    designlab1/designlab1


.. toctree::
  :maxdepth: 2
  :caption: Appendix
  :name: _appendix
  :hidden:

  appendix/glossary

.. _getting_started:

---------------
Getting Started
---------------

This workshop is design for SEs to apply Oracle best practice through a step by step guide. The content is based on Best Practice Guide - Oracle on AHV version 1.3.
Unless, presented with an working opportunity, most technical person's experience of Oracle on AHV is restricted to just reading through the guide but they have yet experiences applying any of the parameters or settings in a working Oracle to see the effects for themselves.
This lab is written to a non-Oracle DBA and requires no prior Oracle/DBA skillsets to handling the lab, it’s a quick way to apply those best practice centering around making tweaks to the operating systems, storage and memory settings of Oracle DB. Although reading up the best practise guide is a pre-requisite, following the lab with further reading of the guide could further strengthen the knowledge and appreciation for tweaking and changing the parameters. 
With the knowledge acquired after this lab, you can apply this to your POC or when a customer needing advice on running Oracle on Nutanix.
This guide does not cover the installation process of installing a Oracle database.
If you want learn how to installed a Oracle database , you can find ”how to” in these links.

- Oracle Official Website :
https://docs.oracle.com/database/121/LADBI/toc.htm

- Un Official Website :
http://www.snapdba.com/2014/01/oracle-database-11gr2-11-2-0-4-installation-on-oracle-linux-6-4/

---------------
Lab Environment
---------------

-Hardware:

  - Lenovo HX or any supported/certified platform Nutanix AOS running

  - Nutanix CE also can be a Lab environment

  - You can download Nutanix CE from here. https://www.nutanix.com/products/community-edition/

-Software :

 - Oracle Linux. You can download from Oracle Website. https://www.oracle.com/linux/index.html . If you are installing Oracle 11gR2, it is recommended to use Oracle Linux 6 but if you are installing Oracle 12cR1 above , it is recommendded to use Oracle Linux 7

 - Oracle database binary. You can download from http://www.oracle.com/technetwork/database/enterprise-edition/downloads/index-092322.html

 - Recommend using 11gR2 database version above for this lab

Setup Lab
+++++++++
To begin from scratch, please foundation your Nutanix blocks (How to Foundation Nutanix Block)
You can watch the video guide from https://www.nutanix.com/2014/07/15/nutanix-foundation-demo-video-from-bare-metal-to-production-in-minutes/

The foundation software is available on

https://portal.nutanix.com/#/page/foundation/list

After finishing the foundation process, you can create a VM that content Oracle Linux OS. Install Oracle database follow this link -

https://www.youtube.com/watch?v=CwHetPzsQBY

Create your base image of VM. After you create this VM , you can clone VMs base on it.
The only thing you need to modify is host name to IP address . Means you need to modify your /etc/hosts point to the right IP address.

If you have any question, you can send a email to albert.chen@nutanix.com. I will happy to teach you how to setup a environment or provide the base VM image to you.
