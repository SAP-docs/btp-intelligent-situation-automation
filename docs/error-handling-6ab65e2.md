<!-- loio6ab65e27124644e4a1c7b05bc04ceefa -->

# Error Handling

If you need support or encounter technical issues while working with Intelligent Situation Automation, you can contact SAP by reporting an incident for component **CA-SIT-ATM**. However, before you report an incident take a look at the following section to too see whether a solution to your error has already been described.



<a name="loio6ab65e27124644e4a1c7b05bc04ceefa__section_hhm_4yk_ypb"/>

## Known Errors and Solutions



<a name="loio6ab65e27124644e4a1c7b05bc04ceefa__section_jff_f5h_zpb"/>

## A server error has occurred. Please try again later.

The user has onboarded but is unable to access the [Manage Situation Automation](https://help.sap.com/viewer/dd7bde0fac4e421bb79830f81df88c86/1.0/en-US/08a87f8a4f95424182f7fc6f8c18c536.html "") :arrow_upper_right: app. This leads to an error.

*Cause*: The user doesn’t have the necessary authorization.

*Solution*: The user needs the roles listed in [Assigning Role Collections to Users](assigning-role-collections-to-users-32a6fbc.md).



<a name="loio6ab65e27124644e4a1c7b05bc04ceefa__section_r4b_4yh_zpb"/>

## Automation was not performed. No action applied.

The user has configured the rule and triggered automation. Automation was not performed. In the [Analyze Situations](https://help.sap.com/viewer/dd7bde0fac4e421bb79830f81df88c86/1.0/en-US/55d4f9e2d0084d2b91596af2fad5b1b2.html "") :arrow_upper_right: app, the *Resolution Flow* on the *Situation Instance Details* page shows *No Action Applied*.

*Cause*: Rule condition might not match the actual data and may have to be enhanced or corrected.

*Solution*: Correct the rule, and then activate and trigger the situation again with the newest data. Older situations will not be re-picked. Instead, they’ll be sent back to manual processing.



<a name="loio6ab65e27124644e4a1c7b05bc04ceefa__section_cv2_123_zpb"/>

## Automation configuration is missing.

A situation is triggered and in the [Analyze Situations](https://help.sap.com/viewer/dd7bde0fac4e421bb79830f81df88c86/1.0/en-US/55d4f9e2d0084d2b91596af2fad5b1b2.html "") :arrow_upper_right: app, on the*Situation Instance Details* page, the *Resolution Flow* shows *No Automation Configuration Found*.

*Cause*: A situation for situation type X is triggered in the SAP S/4HANA Cloud system. However, no automation configuration exists in SAP BTP for that corresponding situation type X.

*Solution*: The user has to create an automation configuration for the corresponding situation type by using the [Manage Situation Automation](https://help.sap.com/viewer/dd7bde0fac4e421bb79830f81df88c86/1.0/en-US/08a87f8a4f95424182f7fc6f8c18c536.html "") :arrow_upper_right: app in SAP BTP.

