<!-- loio89b6037f7a244c29a2dceb637c6392bc -->

# Expose Situation Handling APIs

You can access SAP S/4HANA or SAP S/4HANA Cloud situations from an external system by exposing the corresponding SAP Situation Handling APIs.



<a name="loio89b6037f7a244c29a2dceb637c6392bc__section_cw1_vby_zqb"/>

## SAP S/4HANA Cloud

A key user needs to create and activate a communication arrangement for a communication scenario.

For Intelligent Situation Automation to access SAP S/4HANA Cloud situations, these communication scenarios must be configured in the SAP S/4HANA Cloud system:

-   SAP\_COM\_0345 \(Business Situation Integration\)

-   SAP\_COM\_0376 \(Business Situation Master Data Integration\)


For more information about creating communication arrangements, refer to [Communication Management](https://help.sap.com/viewer/0f69f8fb28ac4bf48d2b57b9637e81fa/latest/en-US/2e84a10c430645a88bdbfaaa23ac9ff7.html).



<a name="loio89b6037f7a244c29a2dceb637c6392bc__section_b34_wby_zqb"/>

## SAP S/4HANA

For SAP S/4HANA systems, the following APIs must be exposed and activated:

-   [Business Situation - Read](https://help.sap.com/docs/SAP_S4HANA_ON-PREMISE/a156fdaa471548bba5cd0bbaaec9b6bd/e31831d5c0934e34a982039cfd389211.html?locale=en-US) 

-   [Business Situation Type - Read](https://help.sap.com/docs/SAP_S4HANA_ON-PREMISE/a156fdaa471548bba5cd0bbaaec9b6bd/251bcc094bb64219adc396d13332ff23.html?locale=en-US) 


For more information, refer to [Activate and Maintain Services](https://help.sap.com/docs/SAP_S4HANA_ON-PREMISE/68bf513362174d54b58cddec28794093/bb2bfe50645c741ae10000000a423f68.html?locale=en-US) and [Activate OData Services for APIs](https://help.sap.com/docs/SAP_S4HANA_ON-PREMISE/8308e6d301d54584a33cd04a9861bc52/6f95c8409ede462996abbae09c3239b2.html?locale=en-US).

Use the cloud connector to allow access from SAP BTP to your SAP S/4HANA system. For more information, refer to [Cloud Connector](https://help.sap.com/viewer/cca91383641e40ffbe03bdc78f00f681/Cloud/en-US/e6c7616abb5710148cfcf3e75d96d596.html).

