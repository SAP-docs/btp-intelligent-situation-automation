<!-- loioe5d5445b80f84fcfab3d49e43b55e563 -->

# Defining and Bundling Roles

Intelligent Situation Automation provides the following role templates:


<table>
<tr>
<th valign="top">

Role Template

</th>
<th valign="top">

Description

</th>
<th valign="top">

Available Attributes

</th>
<th valign="top">

Tiles on SAP Fiori Launchpad

</th>
</tr>
<tr>
<td valign="top">

SituationAutomationKeyUser

</td>
<td valign="top">

Key user for Intelligent Situation Automation

</td>
<td valign="top">

None

</td>
<td valign="top">

-   Manage Situation Actions
-   Manage Situation Automation
-   Situation Dashboard
-   Analyze Situations
-   Delete Data Context
-   Explore Related Situations



</td>
</tr>
<tr>
<td valign="top">

SituationAutomationAdminUser

</td>
<td valign="top">

Admin user for Intelligent Situation Automation 

</td>
<td valign="top">

None

</td>
<td valign="top">

Onboard System

</td>
</tr>
</table>

If the role template doesn't have any attributes, then the corresponding roles are identical to the role templates and are created automatically. If the role template has one or more attributes, you must create roles based on the role templates and provide the attribute values.

As a prerequisite for assigning roles to IdP users or user groups, you also need to configure role collections. A role collection consists of one or more roles from one or more applications and can be used to bundle authorizations within and across applications.

For more information about how to create roles and how to bundle them in role collections using the SAP BTP cockpit, see [Building Roles and Role Collections for Applications](https://help.sap.com/viewer/65de2977205c403bbc107264b8eccf4b/Cloud/en-US/eaa6a26291914b348e875a00b6beb729.html).

