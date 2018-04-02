# xMatters + EasyVista Two Way Integration

# Prerequisites
In order to produce a fully working integration you must have a instance of xMatters and EasyVista and basic familiariy with SQL and JavaScript

# Getting Started
To get started with the integration with EasyVista, you must first [import](https://help.xmatters.com/OnDemand/xmodwelcome/communicationplanbuilder/exportcommplan.htm) the **EasyVista.zip** commmunication plan attatched. 

Once the communication plan is imported, you need to create a group in xMatters (I.E "EasyVistaDemo") and add yourself to that group.

# Configuring EasyVista

To produce a fully working two way integration with xMatters, configuring EasyVista correctly is key. The configuration with EasyVista is a bit more complex comapred to xMatters. Rest assured, we will go through each configuration step by step in this lab.

First and foremost, you must first create an API REST Connection with EasyVista. You can do that by clicking **Administration** < **REST** < **Connections**

<kbd>
    <img src="images/rest.png">
</kbd>


