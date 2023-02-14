<!-- loio44c498e7fca34e4588a03c15e7add82a -->

# Configurations for Resolving Situations Automatically

Situations can be resolved automatically either by using standard actions delivered by SAP or custom actions.



<a name="loio44c498e7fca34e4588a03c15e7add82a__section_ojj_r3y_zqb"/>

## SAP S/4HANA Cloud



### Expose Standard Actions

To enable standard actions, you need to configure destinations for these communication [scenarios](onboarding-bb6b436.md) and situation templates, in your subaccount:


<table>
<tr>
<th valign="top">

Situation Template



</th>
<th valign="top">

Communications Scenario



</th>
</tr>
<tr>
<td valign="top">

Contract is Ready as Source of Supply

\(PROC\_CONTRACTREADYTOUSE\_V3\)



</td>
<td valign="top">

Purchase Requisition Integration

\(SAP\_COM\_0102\)



</td>
</tr>
<tr>
<td valign="top">

Physical Inventory Monitoring

\(MAN\_PHYSICAL\_INVENTORY\_MONITOR\)



</td>
<td valign="top">

Physical Inventory Document Integration

\(SAP\_COM\_0107\)



</td>
</tr>
</table>



<a name="loio44c498e7fca34e4588a03c15e7add82a__section_ohv_y3y_zqb"/>

## SAP S/4HANA



### Expose Standard Actions

To enable standard actions, you need to configure the following destination APIs:


<table>
<tr>
<th valign="top">

Situation Template



</th>
<th valign="top">

APIs



</th>
</tr>
<tr>
<td valign="top">

Contract is Ready as Source of Supply

\(PROC\_CONTRACTREADYTOUSE\_V3\)



</td>
<td valign="top">

 [Purchase Requisition Integration](https://help.sap.com/viewer/91af7f8d3acd47da90d33aaacfcd0d59/latest/en-US/43c43f584eff2160e10000000a44147b.html) 



</td>
</tr>
<tr>
<td valign="top">

Physical Inventory Monitoring

\(MAN\_PHYSICAL\_INVENTORY\_MONITOR\)



</td>
<td valign="top">

 [Physical Inventory Document Integration](https://help.sap.com/viewer/eb2a39dd0c124fed8252f684002d55e1/latest/en-US/58361658745b1f60e10000000a44147b.html) 



</td>
</tr>
</table>



## Custom Actions for Resolving a Situation

You can also resolve a situation with a custom action when you create an automation rule. A custom action can be implemented as a synchronous REST API and a POST request is made with the following payload, which contains information about the situation data context.

> ### Sample Code:  
> ```
> {
>    "input": {
>       "dataContext": "<situation data context json>"
>    }
> }
> ```

> ### Note:  
> When creating an automation configuration, you can see the payload in the parameter section of the custom action.

