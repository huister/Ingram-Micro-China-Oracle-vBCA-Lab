.. Adding labels to the beginning of your lab is helpful for linking to the lab from other pages
.. _example_lab_1:

-------------
Lab 1: Using Swingbench for Oracle Performance Test
-------------

Create Testing Schema
++++++++

Swingbench is a load generator and benchmark tool designed to stress test an Oracle database. It provides OLTP or OLAP testing and is suitable to simulate scenarios where customer could potentially be facing in their own production environment, to use swingbench you can download it here http://dominicgiles.com/swingbench.html
Swingbench is selected for this exercise as part of the partner training not only because it is available for free download, but it is also fairly easy to install, configure and ran the tests cases needed to provide the outcome. 
There are two tasks to be done when we using Swingbench for testing OLTP performance. In the first task, you need to create a Schema (collection of testing tables and indexes ).
Create the schema
Go to **/home/oracle/swingbemch/bin** , execute the **./oewizard** to build your schema.

.. figure:: images/createschema.png

Then you will see the screen below , click **Next** to continue

.. figure:: images/OE1.png

Select Version 2.0 and click **Next**

.. figure:: images/OE2.png

Select **“Create the Order Entry Schema“** and click **“Next”**

.. figure:: images/OE3.png

Change Connect String to **//Hostname/SID** (Depends on your Oracle environment) in this lab is //Linux666/orcl , and the DBA password is qaz12345 (Depends on you Oracle environment), Click **Next**

.. figure:: images/OE4.png

Leave all default values, except for**Tablespace’s Datafile** please enter **+DATA** (Your ASM disk group name) as below show, Click **Next**

.. figure:: images/OE5.png

In **Database Options** window, leave all default values. Click **Next** to proceed.

.. figure:: images/OE6.png

Change the size as **“10GB”**, it will create about 32GB data in this schema , Click **“Next”**

.. figure:: images/OE7.png

Leave all default values and Click “Finish”

.. figure:: images/OE8.png

Schema is creating in progress

.. figure:: images/OE9.png

In **Schema Created** window, invalid entries should show as **None** once the process is completed, click **OK** to proceed. Then your schema is done.

.. figure:: images/OE10.png

Running Swingbench testing
++++++++++++++++++++++++++

The 2nd Task involves executing swingbench tests. 
Go to **/home/oracle/swingbemch/bin** , execute the **./swingbench** to run OLTP testing

.. figure:: images/SW1.png

change the **Connect String** to /Linux666/orcl, Linux666 is hostname , orcl is instance name of Oracle (Adjust by your own environment)

.. figure:: images/SW2.png

Click the connection test button **“the blue earth”**, testing swingbench client can be successful connect to Database

.. figure:: images/SW3.png

change the Number of user to 350 , Benchmark Run Tim to 10 minutes and Record Statistic After 5 minutes

.. figure:: images/SW4.png

Click the **Distributed Controls** tab, and type the Hostname to Linux666 , username use root , and Password is qaz12345. After input , please try **“Test Connection”**


.. figure:: images/SW5.png


.. figure:: images/SW6.png

After all set , please click the **Play** the green button.

.. figure:: images/SW7.png

The you can see swingbench start perform OLTP testing .


.. figure:: images/SW8.png
