<!-- loioe5f9e8172d0340528c6bd1696d321e40 -->

# Authorization and Permissions

Working in *View Analyzer* requires different privileges and permissions to perform different tasks. You will not be able to view entities that you do not have the correct role to access.



<a name="loioe5f9e8172d0340528c6bd1696d321e40__section_u52_mvf_scc"/>

## Unauthorized Notification

When a user does not have permission to access a space or spaces, a row titled *unauthorized* will be displayed.

You can only view enties that you have permsission to see. Entites from spaces that you are not al allowed to view will be labeled as unauthorized. You must ask permission from an administrator for correct authorization to view hidden entities.

> ### Note:  
> To start the *View Analyzer* you will need both the *DW Modeler* and *DW Integrator* scoped roles. You will be able to see all entities with either the global role *DW Administrator* or a custom role that includes *Data Warehouse Runtime \(Read\)* privilege.
> 
> Ask your tenant administrator to assign you a scoped or custom role that fits your required task.

![](images/Cross-space_view_analyzer_8_unauthorized_db36e49.png)

This can also be seen in the lineage graph.

![](images/Cross-space_unauthorized_lineage_9_61a8d4d.png)



<a name="loioe5f9e8172d0340528c6bd1696d321e40__section_l4f_svf_scc"/>

## Permissions

The *View Analyzer* provides you with statistcs and useful information on each entity that composes your view. There are a variety of ways to learn more about your view and make decisions to optimize your data model and performance. Due to the potential sensitivity of information gathered in *View Analyzer*, either the *DW Administrator* role or a custom role is required to run the view or to read the results of generated files.

Ask your tenant administrator to assign you a scoped or custom role that fits your required task.

****


<table>
<tr>
<th valign="top">

Action

</th>
<th valign="top">

Permission

</th>
</tr>
<tr>
<td valign="top">

Run *View Analyzer* without memory consumption

</td>
<td valign="top">

To run *View Analyzer* without memory consumption, you must have a role that is either based on the scroped role *DW Administrator* or on a custom role that includes the *Data Warehouse Data Integration \(Read, Update, Execute\)* and *Data Builder \(Read\)* privleges.

</td>
</tr>
<tr>
<td valign="top">

Run *View Analyzer* with memory consumption

</td>
<td valign="top">

To run the*View Analyzer* with memory consumption you must have a role that is either based on the scoped role *DW Administrator* or a custom role that includes *Data Warehouse Data Integration \(Read, Update, Execute\)* and *Data Builder \(Read\)* and the additional *Space \(Read\)* privilege.

</td>
</tr>
<tr>
<td valign="top">

*Generate SQL Analyzer Plan File* 

</td>
<td valign="top">

You can generate a SQL analyzer plan file with the same permission required to run *View Analyzer* without memory consumption.

To download the SQL analyzer plan file, you must have either the scoped role *DW Administrator* or a custom role that includes *Data Warehouse Runtime \(Read\)* privilege.

</td>
</tr>
</table>

> ### Note:  
> For more information see: [Privileges and Permissions](https://help.sap.com/viewer/935116dd7c324355803d4b85809cec97/DEV_CURRENT/en-US/d7350c6823a14733a7a5727bad8371aa.html "A privilege represents a task or an area in SAP Datasphere and can be assigned to a specific role. The actions that can be performed in the area are determined by the permissions assigned to a privilege.") :arrow_upper_right:
