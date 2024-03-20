<!-- loio39d1b01dde55467492b7c12422a7a212 -->

# Set Up Communication With SAP BTP

New situations created are published as events by the Business Event Handling framework. Intelligent Situation Automation consumes these events by using the SAP Event Mesh service. To enable the exchange of events across different platforms, you need to create an Event Mesh instance.



## Create an Event Mesh Service Instance

Ensure that you have `topicRules` configured so that it can send a message to the topic `saas/isa/cons/*`. Intelligent Situation Automation automatically processes situation events published with this topic.

> ### Note:  
> You need to create the Event Mesh instance in the same subaccount where you've subscribed to Intelligent Situation Automation.

For more information about creating an Event Mesh service instance, see [Create an Event Mesh Service Instance](https://help.sap.com/viewer/bf82e6b26456494cbdd197057c09979f/Cloud/en-US/d0483a9e38434f23a4579d6fcc72654b.html).



## Create an Event Mesh Service Key

After creating a service instance, you need to create a service key for your Event Mesh service instance. The service key helps to connect a SAP S/4HANA or SAP S/4HANA Cloud system to your service instance.

To create a service key, open your service instance, and choose *Service Keys* \> *Create Service Key*.



<a name="loio39d1b01dde55467492b7c12422a7a212__section_k4f_kxk_plb"/>

## Create an Event Channel

You need to use the service key for your Event Mesh service instance to set up an event channel. While creating the channel, ensure `saas/isa/cons` is the *Topic Space*.



### SAP S/4HANA Cloud

Set up the SAP\_COM\_0092 communication scenario. For more information about enabling Enterprise Events, see [Create, Maintain and Delete Communication Arrangements](https://help.sap.com/viewer/0f69f8fb28ac4bf48d2b57b9637e81fa/latest/en-US/214442004da34f738a97f7e924db7fed.html).



### SAP S/4HANA

Refer to [Creating Channels Using a Service Key](https://help.sap.com/docs/SAP_S4HANA_ON-PREMISE/810dfd34f2cc4f39aa8d946b5204fd9c/54b7357a1d0447479f9bf509ca5b24dd.html?locale=en-US).



## Maintain Outbound Event Topic Bindings

In the SAP S/4HANA or SAP S/4HANA Cloud system, bind these topics as the outbound topics for the created channel:

-   `sap/s4/beh/businesssituation/v1/BusinessSituation/*`

-   `sap/s4/beh/businesssituationtype/v1/BusinessSituationType/*`




### SAP S/4HANA Cloud

Refer to [Maintain Outbound Event Topic Bindings for Communication Arrangements](https://help.sap.com/viewer/0f69f8fb28ac4bf48d2b57b9637e81fa/latest/en-US/978b0394caf94e558f488282f68a8bcb.html).



### SAP S/4HANA

Refer to [Maintain Outbound Event Topics](https://help.sap.com/docs/SAP_S4HANA_ON-PREMISE/810dfd34f2cc4f39aa8d946b5204fd9c/bd3cdc18e2d545dc98ecd126e52e8e10.html?locale=en-US).

