# xMatters + EasyVista Two Way Integration

# Prerequisites
In order to produce a fully working integration you must have a instance of xMatters and EasyVista and basic familiariy with SQL and JavaScript

# Getting Started
To get started with the integration with EasyVista, you must first [import](https://help.xmatters.com/OnDemand/xmodwelcome/communicationplanbuilder/exportcommplan.htm) the **EasyVista.zip** commmunication plan attatched. 

Once the communication plan is imported, you need to create a group in xMatters (I.E "EasyVistaDemo") and add yourself to that group.

# Configuring EasyVista

To produce a fully working two way integration with xMatters, configuring EasyVista correctly is key. The configuration with EasyVista is a bit more complex comapred to xMatters. Rest assured, we will go through each configuration step by step in this lab.

### Creating a REST Connection
1. First and foremost, you must first create an API REST Connection with EasyVista. You can do that by clicking **Administration** < **REST** < **Connections**



<kbd>
    <img src="images/rest.png">
</kbd>



Click the **+** button next to **Connections** and add a new connection




<kbd>
    <img src="images/connection.png">
</kbd>



You can call the connection **xM Connection**, the Authentication Method can be **Basic** and in the **Service Url** field, include the name of your instance. User Name Authentication can be any user in xMatters that has the **REST Web Services User** roles. In this example, I have created a user specifically for this demo with the username "easyvista".



<kbd>
    <img src="images/roles.png">
</kbd>


Once this configuration is set up, you can click **Save**

### Creating a Resource

Next, we'll need to create a Resource in EasyVista


3. The next thing we'll need to do is edit your current workflow so EasyVista knows how and when to trigger an event in xMatters. In this example, I am editing the workflow **Incident:Database**. 

To add REST xM Connection we just created, click into **REST ACTIONS** and drag the xM Connection box into the workflow. You can name the workflow whatever you want. Here, I have named it **SendtoXM**.

<kbd>
    <img src="images/workflow_editor.png">
</kbd>



<kbd>
    <img src="images/workflow.png">
</kbd>

