<!-- loio32a6fbcf1464499d9dfdc59c55f4cd7d -->

# Assigning Role Collections to Users

In the SAP BTP cockpit, you must assign role collections to IdP users or user groups. As a prerequisite, users and user groups must have been created in the Identity Authentication service or another IdP.

> ### Note:  
> If you use the SAP ID service, you assign role collections to individual users. If you use the Identity Authentication service or another IdP, you assign them either to individual users or to user groups.

For more information about how to assign role collections to users or user groups using the SAP BTP cockpit, see [Assigning Role Collections to Users or User Groups](https://help.sap.com/docs/BTP/65de2977205c403bbc107264b8eccf4b/31532c77bd61421e9d40d100fd75ef52.html?locale=en-US).

Intelligent Situation Automation uses the standard authentication and authorization procedures provided in the SAP BTP, Cloud Foundry. For more information, see [Authorization and Trust Management in the Cloud Foundry Environment](https://help.sap.com/viewer/65de2977205c403bbc107264b8eccf4b/Cloud/en-US/6373bb7a96114d619bfdfdc6f505d1b9.html).

For Intelligent Situation Automation, you need to:

-   Create a role collection for key users:


    <table>
    <tr>
    <th valign="top">

    Role Template


    
    </th>
    <th valign="top">

    Description


    
    </th>
    </tr>
    <tr>
    <td valign="top">

    RuleRepositorySuperUser


    
    </td>
    <td valign="top">

    Author rules


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    SituationAutomationKeyUser


    
    </td>
    <td valign="top">

    Key user for Intelligent Situation Automation


    
    </td>
    </tr>
    </table>
    
-   Create a role collection for admin user:


    <table>
    <tr>
    <th valign="top">

    Role Template


    
    </th>
    <th valign="top">

    Description


    
    </th>
    </tr>
    <tr>
    <td valign="top">

    SituationAutomationAdminUser


    
    </td>
    <td valign="top">

    Admin user for Intelligent Situation Automation


    
    </td>
    </tr>
    </table>
    

