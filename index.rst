.. title:: Oracle on Nutanix Training

.. toctree::
  :maxdepth: 2
  :caption: Oracle Presentation Deck
  :name: _OracleDeck
  :hidden:

  OracleDeck/aaa


.. toctree::
  :maxdepth: 2
  :caption: Oracle Hands on Labs
  :name: _labs
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

This workshop is for quick apply Oracle best practice step by step base on Nutanix Oralce on AHV best practice for SE or partner training.
I found most of technical persons read the best practice guide but still can’t apply these parameter or settings.
That why I wrote this workshop material for who doesn't have any Oracle technical background but still want apply Oracle best practice on Nutanix for POC or testing purpose.
It’s a quick way to apply those best practice. I still suggest you must read our Nutanix best guide to understand why we need to change some parameters and configuration to get best performance.
After you learned, You can apply this to your POC or when customer want running Oracle on Nutanix.
In this guide , we didn't mention about how to install a Oracle database.
If you want learn how to installed a Oracle database , you can find ”how to” in these links.

- Oracle Official Website :
https://docs.oracle.com/database/121/LADBI/toc.htm

- Un Official Website :
http://www.snapdba.com/2014/01/oracle-database-11gr2-11-2-0-4-installation-on-oracle-linux-6-4/

---------------
Lab Environment
---------------

-Hardware:

  - Nutanix NX ,HX , XC any platform that Nutanix AOS running inside

  - Nutanix CE also can be a Lab environment

  - You can download Nutanix CE from here. https://www.nutanix.com/products/community-edition/

-Software :

 - Oracle Linux. You can download from Oracle Website. https://www.oracle.com/linux/index.html . If you are install Oracle 11gR2, I
 recommend you use Oracle Linux 6. If you are install Oracle 12cR1 above , I will recommend you use Oracle Linux 7

 - Oracle database binary. You can download from http://www.oracle.com/technetwork/database/enterprise-edition/downloads/index-092322.html

 - Recommend using 11gR2 database version above for this lab

Setup Lab
+++++++++
After you foundation your Nutanix blocks (How to Foundation Nutanix Block)
You can watch the video from https://www.nutanix.com/2014/07/15/nutanix-foundation-demo-video-from-bare-metal-to-production-in-minutes/

The foundation software is available on

https://portal.nutanix.com/#/page/foundation/list

After finish foundation, you can create a VM that content Oracle Linux OS. Install Oracle database follow this link -

https://www.youtube.com/watch?v=CwHetPzsQBY

Create your base image of VM. After you create this VM , you can clone VMs base on it.
The only thing you need to modify is host name to IP address . Means you need to modify your /etc/hosts point to the right IP address.

If you have any question, you can send a email to albert.chen@nutanix.com. I will happy to teach you how to setup a environment or provide the base VM image to you.
