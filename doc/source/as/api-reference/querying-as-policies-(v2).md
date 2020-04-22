# Querying AS Policies \(V2\)<a name="EN-US_TOPIC_0103010242"></a>

## Function<a name="section37171354191617"></a>

This interface is used to query AS policies based on search criteria. The results are displayed by page.

-   The difference between the V2 and V1 interfaces for querying AS policies is that V2 contains scaling resource types in response messages.
-   Search criteria can be the AS policy name, policy type, policy ID, start line number, and number of records.
-   If no search criteria are specified, a maximum of 20 AS policies for specified resources can be queried for a tenant by default.

## URI<a name="section43911613201715"></a>

GET /autoscaling-api/v2/\{project\_id\}/scaling\_policy/\{scaling\_resource\_id\}/list

>![](public_sys-resources/icon-note.gif) **NOTE:**   
>You can type the question mark \(?\) and ampersand \(&\) at the end of the URI to define multiple search criteria. AS policies can be searched by all optional parameters in the following table. For details, see the example request.  

**Table  1**  Parameter description

<a name="table1888013021719"></a>
<table><thead align="left"><tr id="row129771730161718"><th class="cellrowborder" valign="top" width="18.81188118811881%" id="mcps1.2.5.1.1"><p id="p0977153081716"><a name="p0977153081716"></a><a name="p0977153081716"></a><strong id="b1634182125612"><a name="b1634182125612"></a><a name="b1634182125612"></a>Parameter</strong></p>
</th>
<th class="cellrowborder" valign="top" width="19.801980198019802%" id="mcps1.2.5.1.2"><p id="p69771430141713"><a name="p69771430141713"></a><a name="p69771430141713"></a>Mandatory</p>
</th>
<th class="cellrowborder" valign="top" width="13.861386138613863%" id="mcps1.2.5.1.3"><p id="p20977193012175"><a name="p20977193012175"></a><a name="p20977193012175"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="47.524752475247524%" id="mcps1.2.5.1.4"><p id="p797703041713"><a name="p797703041713"></a><a name="p797703041713"></a><strong id="b18731132116565"><a name="b18731132116565"></a><a name="b18731132116565"></a>Description</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="row1097753041715"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p1497773017172"><a name="p1497773017172"></a><a name="p1497773017172"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p597763017179"><a name="p597763017179"></a><a name="p597763017179"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.3 "><p id="p197793017178"><a name="p197793017178"></a><a name="p197793017178"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.2.5.1.4 "><p id="p36520930"><a name="p36520930"></a><a name="p36520930"></a>Specifies the project ID.</p>
</td>
</tr>
<tr id="row4977130111714"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p3977130181718"><a name="p3977130181718"></a><a name="p3977130181718"></a>scaling_resource_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p7977113021713"><a name="p7977113021713"></a><a name="p7977113021713"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.3 "><p id="p597718304170"><a name="p597718304170"></a><a name="p597718304170"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.2.5.1.4 "><p id="p1897713013179"><a name="p1897713013179"></a><a name="p1897713013179"></a>Specifies the scaling resource ID.</p>
</td>
</tr>
<tr id="row159778304174"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p199771130131719"><a name="p199771130131719"></a><a name="p199771130131719"></a>scaling_policy_name</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p2977113021715"><a name="p2977113021715"></a><a name="p2977113021715"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.3 "><p id="p14977183011717"><a name="p14977183011717"></a><a name="p14977183011717"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.2.5.1.4 "><p id="p197763018172"><a name="p197763018172"></a><a name="p197763018172"></a>Specifies the AS policy name.</p>
<p id="p1699918201016"><a name="p1699918201016"></a><a name="p1699918201016"></a>Supports fuzzy search. </p>
</td>
</tr>
<tr id="row4977133071716"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p2977163031717"><a name="p2977163031717"></a><a name="p2977163031717"></a>scaling_policy_type</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p149771130101718"><a name="p149771130101718"></a><a name="p149771130101718"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.3 "><p id="p1797733021713"><a name="p1797733021713"></a><a name="p1797733021713"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.2.5.1.4 "><p id="p1397713306171"><a name="p1397713306171"></a><a name="p1397713306171"></a>Specifies the AS policy type.</p>
<a name="ul1459175775513"></a><a name="ul1459175775513"></a><ul id="ul1459175775513"><li><strong id="b111815744210"><a name="b111815744210"></a><a name="b111815744210"></a>ALARM</strong>: alarm policy</li><li><strong id="b7228155915425"><a name="b7228155915425"></a><a name="b7228155915425"></a>SCHEDULED</strong>: scheduled policy</li><li><strong id="b38941900437"><a name="b38941900437"></a><a name="b38941900437"></a>RECURRENCE</strong>: periodic policy</li></ul>
</td>
</tr>
<tr id="row39536973112658"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p5764343811270"><a name="p5764343811270"></a><a name="p5764343811270"></a>scaling_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p3860687711270"><a name="p3860687711270"></a><a name="p3860687711270"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.3 "><p id="p4014932111270"><a name="p4014932111270"></a><a name="p4014932111270"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.2.5.1.4 "><p id="p3086952911270"><a name="p3086952911270"></a><a name="p3086952911270"></a>Specifies the AS policy ID.</p>
</td>
</tr>
<tr id="row1997753012173"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p20977153015171"><a name="p20977153015171"></a><a name="p20977153015171"></a>start_number</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p19977123051713"><a name="p19977123051713"></a><a name="p19977123051713"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.3 "><p id="p129771430121718"><a name="p129771430121718"></a><a name="p129771430121718"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.2.5.1.4 "><p id="p59373825"><a name="p59373825"></a><a name="p59373825"></a>Specifies the start line number. The default value is <strong id="b56977494586"><a name="b56977494586"></a><a name="b56977494586"></a>0</strong>. The minimum parameter value is <strong id="b18744142621611"><a name="b18744142621611"></a><a name="b18744142621611"></a>0</strong>.</p>
</td>
</tr>
<tr id="row8977123031717"><td class="cellrowborder" valign="top" width="18.81188118811881%" headers="mcps1.2.5.1.1 "><p id="p11978630121710"><a name="p11978630121710"></a><a name="p11978630121710"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="19.801980198019802%" headers="mcps1.2.5.1.2 "><p id="p149781030191713"><a name="p149781030191713"></a><a name="p149781030191713"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="13.861386138613863%" headers="mcps1.2.5.1.3 "><p id="p17978230141711"><a name="p17978230141711"></a><a name="p17978230141711"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="47.524752475247524%" headers="mcps1.2.5.1.4 "><p id="p21968676"><a name="p21968676"></a><a name="p21968676"></a>Specifies the number of query records. The default value is <strong id="b168447885495335"><a name="b168447885495335"></a><a name="b168447885495335"></a>20</strong>. The value range is 0 to 100.</p>
</td>
</tr>
</tbody>
</table>

## Request Message<a name="section1229531121814"></a>

-   Request parameters

    None

-   Example request

    This example shows how to query all periodic AS policies for resources with ID  **8ade64b5-d685-40b8-8582-4ce306ea37a6**.

    ```
    GET https://{Endpoint}/autoscaling-api/v2/{project_id}/scaling_policy/8ade64b5-d685-40b8-8582-4ce306ea37a6/list?scaling_policy_type=RECURRENCE
    ```


## Response Message<a name="section1399662217181"></a>

-   Response parameters

    **Table  2**  Response parameters

    <a name="table8998622101819"></a>
    <table><thead align="left"><tr id="row16792317182"><th class="cellrowborder" valign="top" width="26.567343265673433%" id="mcps1.2.4.1.1"><p id="p11677233185"><a name="p11677233185"></a><a name="p11677233185"></a><strong id="b175351324125618"><a name="b175351324125618"></a><a name="b175351324125618"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="18.298170182981703%" id="mcps1.2.4.1.2"><p id="p8676234180"><a name="p8676234180"></a><a name="p8676234180"></a><strong id="b84235270693914"><a name="b84235270693914"></a><a name="b84235270693914"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="55.134486551344864%" id="mcps1.2.4.1.3"><p id="p467123161819"><a name="p467123161819"></a><a name="p467123161819"></a><strong id="b11992182516566"><a name="b11992182516566"></a><a name="b11992182516566"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row18671239186"><td class="cellrowborder" valign="top" width="26.567343265673433%" headers="mcps1.2.4.1.1 "><p id="p1567182318187"><a name="p1567182318187"></a><a name="p1567182318187"></a>total_number</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.298170182981703%" headers="mcps1.2.4.1.2 "><p id="p8676231189"><a name="p8676231189"></a><a name="p8676231189"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.134486551344864%" headers="mcps1.2.4.1.3 "><p id="p116752316182"><a name="p116752316182"></a><a name="p116752316182"></a>Specifies the total number of query records.</p>
    </td>
    </tr>
    <tr id="row1067142391818"><td class="cellrowborder" valign="top" width="26.567343265673433%" headers="mcps1.2.4.1.1 "><p id="p196792321817"><a name="p196792321817"></a><a name="p196792321817"></a>start_number</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.298170182981703%" headers="mcps1.2.4.1.2 "><p id="p667523181815"><a name="p667523181815"></a><a name="p667523181815"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.134486551344864%" headers="mcps1.2.4.1.3 "><p id="p146792310186"><a name="p146792310186"></a><a name="p146792310186"></a>Specifies the start line number.</p>
    </td>
    </tr>
    <tr id="row126742391816"><td class="cellrowborder" valign="top" width="26.567343265673433%" headers="mcps1.2.4.1.1 "><p id="p1067112331818"><a name="p1067112331818"></a><a name="p1067112331818"></a>limit</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.298170182981703%" headers="mcps1.2.4.1.2 "><p id="p8678237182"><a name="p8678237182"></a><a name="p8678237182"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.134486551344864%" headers="mcps1.2.4.1.3 "><p id="p5671723171810"><a name="p5671723171810"></a><a name="p5671723171810"></a>Specifies the maximum number of resources to be queried.</p>
    </td>
    </tr>
    <tr id="row867223111812"><td class="cellrowborder" valign="top" width="26.567343265673433%" headers="mcps1.2.4.1.1 "><p id="p11671823161819"><a name="p11671823161819"></a><a name="p11671823161819"></a>scaling_policies</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.298170182981703%" headers="mcps1.2.4.1.2 "><p id="p867152313180"><a name="p867152313180"></a><a name="p867152313180"></a>Array</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.134486551344864%" headers="mcps1.2.4.1.3 "><p id="p9671523171818"><a name="p9671523171818"></a><a name="p9671523171818"></a>Specifies AS policies. For details, see <a href="#table19638345141818">Table 3</a>.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **Table  3** **scaling\_policies**  field description

    <a name="table19638345141818"></a>
    <table><thead align="left"><tr id="row9776134561813"><th class="cellrowborder" valign="top" width="26.529999999999998%" id="mcps1.2.4.1.1"><p id="p2776164561819"><a name="p2776164561819"></a><a name="p2776164561819"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.37%" id="mcps1.2.4.1.2"><p id="p17776154514184"><a name="p17776154514184"></a><a name="p17776154514184"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.1%" id="mcps1.2.4.1.3"><p id="p4776124513183"><a name="p4776124513183"></a><a name="p4776124513183"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1477694516189"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p197761545171810"><a name="p197761545171810"></a><a name="p197761545171810"></a>scaling_policy_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p18776184551815"><a name="p18776184551815"></a><a name="p18776184551815"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p37761945121812"><a name="p37761945121812"></a><a name="p37761945121812"></a>Specifies the AS policy name.</p>
    <p id="p117971094113"><a name="p117971094113"></a><a name="p117971094113"></a>Supports fuzzy search. </p>
    </td>
    </tr>
    <tr id="row137762045161819"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p137763456187"><a name="p137763456187"></a><a name="p137763456187"></a>scaling_policy_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p177761045151815"><a name="p177761045151815"></a><a name="p177761045151815"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p377634541812"><a name="p377634541812"></a><a name="p377634541812"></a>Specifies the AS policy ID.</p>
    </td>
    </tr>
    <tr id="row277610458185"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p1077684513189"><a name="p1077684513189"></a><a name="p1077684513189"></a>scaling_resource_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p1377619452186"><a name="p1377619452186"></a><a name="p1377619452186"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p1977664591811"><a name="p1977664591811"></a><a name="p1977664591811"></a>Specifies the scaling resource ID.</p>
    </td>
    </tr>
    <tr id="row37761845151820"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p127761245131820"><a name="p127761245131820"></a><a name="p127761245131820"></a>scaling_resource_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p1977634511814"><a name="p1977634511814"></a><a name="p1977634511814"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p8776164561818"><a name="p8776164561818"></a><a name="p8776164561818"></a>Specifies the scaling resource type.</p>
    <a name="ul207763456181"></a><a name="ul207763456181"></a><ul id="ul207763456181"><li>AS group: <strong id="b84235270691950"><a name="b84235270691950"></a><a name="b84235270691950"></a>SCALING_GROUP</strong></li><li>Bandwidth: <strong id="b8423527069204"><a name="b8423527069204"></a><a name="b8423527069204"></a>BANDWIDTH</strong></li></ul>
    </td>
    </tr>
    <tr id="row157761645151813"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p1777684591815"><a name="p1777684591815"></a><a name="p1777684591815"></a>policy_status</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p477664511186"><a name="p477664511186"></a><a name="p477664511186"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p177610451188"><a name="p177610451188"></a><a name="p177610451188"></a>Specifies the AS policy status.</p>
    <a name="ul10776124531820"></a><a name="ul10776124531820"></a><ul id="ul10776124531820"><li><strong id="b912511617441"><a name="b912511617441"></a><a name="b912511617441"></a>INSERVICE</strong>: The AS policy is enabled.</li><li><strong id="b144651119164416"><a name="b144651119164416"></a><a name="b144651119164416"></a>PAUSED</strong>: The AS policy is disabled.</li><li><strong id="b842352706171746"><a name="b842352706171746"></a><a name="b842352706171746"></a>EXECUTING</strong>: The AS policy is being executed.</li></ul>
    </td>
    </tr>
    <tr id="row14776124581811"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p1577614459188"><a name="p1577614459188"></a><a name="p1577614459188"></a>scaling_policy_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p19777645161811"><a name="p19777645161811"></a><a name="p19777645161811"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p18777104513185"><a name="p18777104513185"></a><a name="p18777104513185"></a>Specifies the AS policy type.</p>
    <a name="ul277744521819"></a><a name="ul277744521819"></a><ul id="ul277744521819"><li><strong>ALARM</strong>: indicates that the scaling action is triggered by an alarm. A value is returned for <strong>alarm_id</strong>, and no value is returned for <strong>scheduled_policy</strong>.</li><li><strong id="b842352706174318"><a name="b842352706174318"></a><a name="b842352706174318"></a>SCHEDULED</strong>: indicates that the scaling action is triggered as scheduled. A value is returned for <strong id="b842352706174359"><a name="b842352706174359"></a><a name="b842352706174359"></a>scheduled_policy</strong>, and no value is returned for <strong id="b842352706174456"><a name="b842352706174456"></a><a name="b842352706174456"></a>alarm_id</strong>, <strong id="b84235270617451"><a name="b84235270617451"></a><a name="b84235270617451"></a>recurrence_type</strong>, <strong id="b84235270617457"><a name="b84235270617457"></a><a name="b84235270617457"></a>recurrence_value</strong>, <strong id="b842352706174512"><a name="b842352706174512"></a><a name="b842352706174512"></a>start_time</strong>, or <strong id="b842352706174516"><a name="b842352706174516"></a><a name="b842352706174516"></a>end_time</strong>.</li><li><strong id="b515011687"><a name="b515011687"></a><a name="b515011687"></a>RECURRENCE</strong>: indicates that the scaling action is triggered periodically. Values are returned for <strong id="b1180446588"><a name="b1180446588"></a><a name="b1180446588"></a>scheduled_policy</strong>, <strong id="b1121671907174638"><a name="b1121671907174638"></a><a name="b1121671907174638"></a>recurrence_type</strong>, <strong id="b413073752174638"><a name="b413073752174638"></a><a name="b413073752174638"></a>recurrence_value</strong>, <strong id="b1481332545174638"><a name="b1481332545174638"></a><a name="b1481332545174638"></a>start_time</strong>, and <strong id="b331387069174638"><a name="b331387069174638"></a><a name="b331387069174638"></a>end_time</strong>, and no value is returned for <strong id="b1373870306"><a name="b1373870306"></a><a name="b1373870306"></a>alarm_id</strong>.</li></ul>
    </td>
    </tr>
    <tr id="row177771245121819"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p10777645151812"><a name="p10777645151812"></a><a name="p10777645151812"></a>alarm_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p1977794531814"><a name="p1977794531814"></a><a name="p1977794531814"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p19777154571815"><a name="p19777154571815"></a><a name="p19777154571815"></a>Specifies the alarm ID.</p>
    </td>
    </tr>
    <tr id="row13777445181812"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p1177710451181"><a name="p1177710451181"></a><a name="p1177710451181"></a>scheduled_policy</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="a4c03d226ca78442f99e13b8d363cd51d"><a name="a4c03d226ca78442f99e13b8d363cd51d"></a><a name="a4c03d226ca78442f99e13b8d363cd51d"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p1377784521818"><a name="p1377784521818"></a><a name="p1377784521818"></a>Specifies the periodic or scheduled AS policy. For details, see <a href="#table1276581101919">Table 4</a>.</p>
    </td>
    </tr>
    <tr id="row8777124516185"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p1577764541819"><a name="p1577764541819"></a><a name="p1577764541819"></a>scaling_policy_action</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p195071335164217"><a name="p195071335164217"></a><a name="p195071335164217"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p187778457184"><a name="p187778457184"></a><a name="p187778457184"></a>Specifies the scaling action of the AS policy. For details, see <a href="#table881433612199">Table 5</a>.</p>
    </td>
    </tr>
    <tr id="row777764515184"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p15777114510187"><a name="p15777114510187"></a><a name="p15777114510187"></a>cool_down_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p12777164521814"><a name="p12777164521814"></a><a name="p12777164521814"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p07771845111814"><a name="p07771845111814"></a><a name="p07771845111814"></a>Specifies the cooldown period (s).</p>
    </td>
    </tr>
    <tr id="row17777144512183"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p277715453186"><a name="p277715453186"></a><a name="p277715453186"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p1677744531814"><a name="p1677744531814"></a><a name="p1677744531814"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p16777145101819"><a name="p16777145101819"></a><a name="p16777145101819"></a>Specifies the time when an AS policy was created. The time format complies with UTC.</p>
    </td>
    </tr>
    <tr id="row1675315217589"><td class="cellrowborder" valign="top" width="26.529999999999998%" headers="mcps1.2.4.1.1 "><p id="p65915113175834"><a name="p65915113175834"></a><a name="p65915113175834"></a>meta_data</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.37%" headers="mcps1.2.4.1.2 "><p id="p1923173718423"><a name="p1923173718423"></a><a name="p1923173718423"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.1%" headers="mcps1.2.4.1.3 "><p id="p41667816175834"><a name="p41667816175834"></a><a name="p41667816175834"></a>Provides additional information. For details, see <a href="#table14568680175854">Table 6</a>.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **Table  4** **scheduled\_policy**  field description

    <a name="table1276581101919"></a>
    <table><thead align="left"><tr id="row10872131111198"><th class="cellrowborder" valign="top" width="26.26%" id="mcps1.2.4.1.1"><p id="p18725111193"><a name="p18725111193"></a><a name="p18725111193"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.2"><p id="p887216111194"><a name="p887216111194"></a><a name="p887216111194"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.559999999999995%" id="mcps1.2.4.1.3"><p id="p16872611141910"><a name="p16872611141910"></a><a name="p16872611141910"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15872181121915"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p1387241171913"><a name="p1387241171913"></a><a name="p1387241171913"></a>launch_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p4872141181919"><a name="p4872141181919"></a><a name="p4872141181919"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p587221118190"><a name="p587221118190"></a><a name="p587221118190"></a>Specifies the time when the scaling action is triggered. The time format complies with UTC.</p>
    <a name="ul19872111121914"></a><a name="ul19872111121914"></a><ul id="ul19872111121914"><li>If <strong>scaling_policy_type</strong> is set to <strong>SCHEDULED</strong>, the time format is <strong>YYYY-MM-DDThh:mmZ</strong>.</li><li>If <strong>scaling_policy_type</strong> is set to <strong>RECURRENCE</strong>, the time format is <strong>hh:mm</strong>.</li></ul>
    </td>
    </tr>
    <tr id="row118721911171915"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p1687216114198"><a name="p1687216114198"></a><a name="p1687216114198"></a>recurrence_type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p168721111131918"><a name="p168721111131918"></a><a name="p168721111131918"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p20872161114196"><a name="p20872161114196"></a><a name="p20872161114196"></a>Specifies the type of a periodically triggered scaling action.</p>
    <a name="ul147782163412"></a><a name="ul147782163412"></a><ul id="ul147782163412"><li><strong id="b175944210506"><a name="b175944210506"></a><a name="b175944210506"></a>Daily</strong>: indicates that the scaling action is triggered once a day.</li><li><strong>Weekly</strong>: indicates that the scaling action is triggered once a week.</li><li><strong>Monthly</strong>: indicates that the scaling action is triggered once a month.</li></ul>
    </td>
    </tr>
    <tr id="row12873161115197"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p887314111190"><a name="p887314111190"></a><a name="p887314111190"></a>recurrence_value</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p11873151151916"><a name="p11873151151916"></a><a name="p11873151151916"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p1387316117199"><a name="p1387316117199"></a><a name="p1387316117199"></a>Specifies the frequency at which scaling actions are triggered.</p>
    <a name="ul1287310117195"></a><a name="ul1287310117195"></a><ul id="ul1287310117195"><li>If <strong id="b7719727185013"><a name="b7719727185013"></a><a name="b7719727185013"></a>recurrence_type</strong> is set to <strong id="b87211127155012"><a name="b87211127155012"></a><a name="b87211127155012"></a>Daily</strong>, the value is <strong id="b5722182719504"><a name="b5722182719504"></a><a name="b5722182719504"></a>null</strong>, indicating that the scaling action is triggered once a day.</li><li>If <strong>recurrence_type</strong> is set to <strong>Weekly</strong>, the value ranges from <strong>1</strong> (Sunday) to <strong>7</strong> (Saturday). The digits refer to dates in each week and separated by a comma, such as <strong>1,3,5</strong>.</li><li>If <strong id="b84235270617528"><a name="b84235270617528"></a><a name="b84235270617528"></a>recurrence_type</strong> is set to <strong>Monthly</strong>, the value ranges from <strong>1</strong> to <strong>31</strong>. The digits refer to the dates in each month and separated by a comma, such as <strong>1,10,13,28</strong>.</li></ul>
    </td>
    </tr>
    <tr id="row1873711201914"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p18873191171918"><a name="p18873191171918"></a><a name="p18873191171918"></a>start_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p587311112194"><a name="p587311112194"></a><a name="p587311112194"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p18736112192"><a name="p18736112192"></a><a name="p18736112192"></a>Specifies the start time of the scaling action triggered periodically. The time format complies with UTC.</p>
    <p id="p19873131110192"><a name="p19873131110192"></a><a name="p19873131110192"></a>The time format is <strong>YYYY-MM-DDThh:mmZ</strong>.</p>
    </td>
    </tr>
    <tr id="row2087371101913"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p1487341151917"><a name="p1487341151917"></a><a name="p1487341151917"></a>end_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p1887318115191"><a name="p1887318115191"></a><a name="p1887318115191"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p16873161110197"><a name="p16873161110197"></a><a name="p16873161110197"></a>Specifies the end time of the scaling action triggered periodically. The time format complies with UTC.</p>
    <p id="p2873201171914"><a name="p2873201171914"></a><a name="p2873201171914"></a>The time format is <strong>YYYY-MM-DDThh:mmZ</strong>.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **Table  5** **scaling\_policy\_action**  field description

    <a name="table881433612199"></a>
    <table><thead align="left"><tr id="row12867203681919"><th class="cellrowborder" valign="top" width="26.26%" id="mcps1.2.4.1.1"><p id="p9867153619195"><a name="p9867153619195"></a><a name="p9867153619195"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="18.18%" id="mcps1.2.4.1.2"><p id="p11867436161911"><a name="p11867436161911"></a><a name="p11867436161911"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="55.559999999999995%" id="mcps1.2.4.1.3"><p id="p4867436161920"><a name="p4867436161920"></a><a name="p4867436161920"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row2867133681914"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p19867123613195"><a name="p19867123613195"></a><a name="p19867123613195"></a>operation</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p1868113616194"><a name="p1868113616194"></a><a name="p1868113616194"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p486863681911"><a name="p486863681911"></a><a name="p486863681911"></a>Specifies the scaling action.</p>
    <a name="ul688316920419"></a><a name="ul688316920419"></a><ul id="ul688316920419"><li><strong id="b8423527069234"><a name="b8423527069234"></a><a name="b8423527069234"></a>ADD</strong>: indicates adding instances.</li><li><strong id="b84235270692351"><a name="b84235270692351"></a><a name="b84235270692351"></a>REDUCE</strong>: indicates reducing instances.</li><li><strong id="b84235270692418"><a name="b84235270692418"></a><a name="b84235270692418"></a>SET</strong>: indicates setting the number of instances to a specified value.</li></ul>
    </td>
    </tr>
    <tr id="row1286813618199"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p886863614192"><a name="p886863614192"></a><a name="p886863614192"></a>size</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p158681836101918"><a name="p158681836101918"></a><a name="p158681836101918"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p58681436191915"><a name="p58681436191915"></a><a name="p58681436191915"></a>Specifies the number of instances to be operated.</p>
    </td>
    </tr>
    <tr id="row086812368197"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p386843661912"><a name="p386843661912"></a><a name="p386843661912"></a>percentage</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p1286883601910"><a name="p1286883601910"></a><a name="p1286883601910"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p6868193614193"><a name="p6868193614193"></a><a name="p6868193614193"></a>Specifies the percentage of instances to be operated.</p>
    </td>
    </tr>
    <tr id="row88685367199"><td class="cellrowborder" valign="top" width="26.26%" headers="mcps1.2.4.1.1 "><p id="p108681036111910"><a name="p108681036111910"></a><a name="p108681036111910"></a>limits</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.18%" headers="mcps1.2.4.1.2 "><p id="p2868936171912"><a name="p2868936171912"></a><a name="p2868936171912"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="55.559999999999995%" headers="mcps1.2.4.1.3 "><p id="p08682369195"><a name="p08682369195"></a><a name="p08682369195"></a>Specifies the operation restrictions.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **Table  6** **meta\_data**  field description

    <a name="table14568680175854"></a>
    <table><thead align="left"><tr id="row25036975175854"><th class="cellrowborder" valign="top" width="23.762376237623762%" id="mcps1.2.4.1.1"><p id="p4598303175854"><a name="p4598303175854"></a><a name="p4598303175854"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="24.752475247524753%" id="mcps1.2.4.1.2"><p id="p36918294175854"><a name="p36918294175854"></a><a name="p36918294175854"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.48514851485149%" id="mcps1.2.4.1.3"><p id="p37591800175854"><a name="p37591800175854"></a><a name="p37591800175854"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row15117177175854"><td class="cellrowborder" valign="top" width="23.762376237623762%" headers="mcps1.2.4.1.1 "><p id="p14729123175854"><a name="p14729123175854"></a><a name="p14729123175854"></a>Additional field key-value pair</p>
    </td>
    <td class="cellrowborder" valign="top" width="24.752475247524753%" headers="mcps1.2.4.1.2 "><p id="p52208315175854"><a name="p52208315175854"></a><a name="p52208315175854"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.48514851485149%" headers="mcps1.2.4.1.3 "><p id="p1015136175854"><a name="p1015136175854"></a><a name="p1015136175854"></a>Specifies the key and value of the metadata.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Example response

    ```
    {
        "limit": 20,
        "total_number": 3,
        "start_number": 0,
        "scaling_policies": [
            {
                "scaling_policy_id": "803a35a5-38fb-4d27-a042-496c14bc1fb8",
                "scaling_policy_name": "as-policy-7a75",
                "scaling_resource_id": "8ade64b5-d685-40b8-8582-4ce306ea37a6",
                "scaling_resource_type": "SCALING_GROUP",
                "scaling_policy_type": "RECURRENCE",
                "scheduled_policy": {
                    "launch_time": "03:30",
                    "recurrence_type": "Daily",
                    "start_time": "2017-08-28T03:08Z",
                    "end_time": "2017-09-01T03:08Z"
                },
                "cool_down_time": 900,
                "scaling_policy_action": {
                    "operation": "ADD",
                    "size": 1
                },
                "policy_status": "INSERVICE",
                "create_time": "2017-08-31T03:02:41Z"
            },
            {
                "scaling_policy_id": "535fd67e-276b-409c-879e-52f4e09e14bb",
                "scaling_policy_name": "as-policy-7a75",
                "scaling_resource_id": "8ade64b5-d685-40b8-8582-4ce306ea37a6",
                "scaling_resource_type": "SCALING_GROUP",
                "scaling_policy_type": "RECURRENCE",
                "scheduled_policy": {
                    "launch_time": "21:30",
                    "recurrence_type": "Daily",
                    "start_time": "2017-08-27T21:08Z",
                    "end_time": "2017-08-31T21:08Z"
                },
                "cool_down_time": 900,
                "scaling_policy_action": {
                    "operation": "ADD",
                    "size": 1
                },
                "policy_status": "INSERVICE",
                "create_time": "2017-08-31T07:35:05Z"
            },
            {
                "scaling_policy_id": "37df92f8-73cb-469e-a420-c15f445d2ee1",
                "scaling_policy_name": "as-policy-7a75",
                "scaling_resource_id": "8ade64b5-d685-40b8-8582-4ce306ea37a6",
                "scaling_resource_type": "SCALING_GROUP",
                "scaling_policy_type": "RECURRENCE",
                "scheduled_policy": {
                    "launch_time": "22:30",
                    "recurrence_type": "Daily",
                    "start_time": "2017-08-27T22:08Z",
                    "end_time": "2017-08-31T22:08Z"
                },
                "cool_down_time": 900,
                "scaling_policy_action": {
                    "operation": "ADD",
                    "size": 1
                },
                "policy_status": "INSERVICE",
                "create_time": "2017-08-31T07:41:06Z"
            }
        ]
    }
    ```


## Returned Values<a name="section2092105419207"></a>

-   Normal

    200

-   Abnormal

    <a name="table152011321112110"></a>
    <table><thead align="left"><tr id="row22672212214"><th class="cellrowborder" valign="top" width="46.46%" id="mcps1.1.3.1.1"><p id="p5267122192117"><a name="p5267122192117"></a><a name="p5267122192117"></a>Returned Values</p>
    </th>
    <th class="cellrowborder" valign="top" width="53.54%" id="mcps1.1.3.1.2"><p id="p1926717218218"><a name="p1926717218218"></a><a name="p1926717218218"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row1626782162110"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p1726782113217"><a name="p1726782113217"></a><a name="p1726782113217"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p3267122110213"><a name="p3267122110213"></a><a name="p3267122110213"></a>The server failed to process the request.</p>
    </td>
    </tr>
    <tr id="row42671421112117"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p142675216217"><a name="p142675216217"></a><a name="p142675216217"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p1267192152120"><a name="p1267192152120"></a><a name="p1267192152120"></a>You must enter the username and password to access the requested page.</p>
    </td>
    </tr>
    <tr id="row13268621102119"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p22682218219"><a name="p22682218219"></a><a name="p22682218219"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p126822112216"><a name="p126822112216"></a><a name="p126822112216"></a>You are forbidden to access the requested page.</p>
    </td>
    </tr>
    <tr id="row13268421202111"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p2026813215215"><a name="p2026813215215"></a><a name="p2026813215215"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p12683210216"><a name="p12683210216"></a><a name="p12683210216"></a>The server could not find the requested page.</p>
    </td>
    </tr>
    <tr id="row17268172122117"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p182681321112114"><a name="p182681321112114"></a><a name="p182681321112114"></a>405 Method Not Allowed</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p5268142110211"><a name="p5268142110211"></a><a name="p5268142110211"></a>You are not allowed to use the method specified in the request.</p>
    </td>
    </tr>
    <tr id="row112684216211"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p19268182115210"><a name="p19268182115210"></a><a name="p19268182115210"></a>406 Not Acceptable</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p6268192113218"><a name="p6268192113218"></a><a name="p6268192113218"></a>The response generated by the server could not be accepted by the client.</p>
    </td>
    </tr>
    <tr id="row926817214212"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p326852113212"><a name="p326852113212"></a><a name="p326852113212"></a>407 Proxy Authentication Required</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p12268172192112"><a name="p12268172192112"></a><a name="p12268172192112"></a>You must use the proxy server for authentication so that the request can be processed.</p>
    </td>
    </tr>
    <tr id="row172681421202119"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p9268132115212"><a name="p9268132115212"></a><a name="p9268132115212"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p926872192111"><a name="p926872192111"></a><a name="p926872192111"></a>The request timed out.</p>
    </td>
    </tr>
    <tr id="row19268142119216"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p9268162119219"><a name="p9268162119219"></a><a name="p9268162119219"></a>409 Conflict</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p52681121162111"><a name="p52681121162111"></a><a name="p52681121162111"></a>The request could not be processed due to a conflict.</p>
    </td>
    </tr>
    <tr id="row13268321112112"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p16268202172111"><a name="p16268202172111"></a><a name="p16268202172111"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p326802120216"><a name="p326802120216"></a><a name="p326802120216"></a>Failed to complete the request because of an internal service error.</p>
    </td>
    </tr>
    <tr id="row10268821172110"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p2268172112211"><a name="p2268172112211"></a><a name="p2268172112211"></a>501 Not Implemented</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p1626918212211"><a name="p1626918212211"></a><a name="p1626918212211"></a>Failed to complete the request because the server does not support the requested function.</p>
    </td>
    </tr>
    <tr id="row19269421192117"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p6269321122113"><a name="p6269321122113"></a><a name="p6269321122113"></a>502 Bad Gateway</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p92691421182110"><a name="p92691421182110"></a><a name="p92691421182110"></a>Failed to complete the request because the request is invalid.</p>
    </td>
    </tr>
    <tr id="row1426920217211"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p3269132118215"><a name="p3269132118215"></a><a name="p3269132118215"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p1126942116217"><a name="p1126942116217"></a><a name="p1126942116217"></a>Failed to complete the request because the system is unavailable.</p>
    </td>
    </tr>
    <tr id="row42690212219"><td class="cellrowborder" valign="top" width="46.46%" headers="mcps1.1.3.1.1 "><p id="p17269102112120"><a name="p17269102112120"></a><a name="p17269102112120"></a>504 Gateway Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="53.54%" headers="mcps1.1.3.1.2 "><p id="p17269182113216"><a name="p17269182113216"></a><a name="p17269182113216"></a>A gateway timeout error occurred.</p>
    </td>
    </tr>
    </tbody>
    </table>


## Error Codes<a name="section17669131616110"></a>

See  [Error Codes](error-codes.md).

