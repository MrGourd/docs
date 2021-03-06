# Querying Security Groups<a name="vpc_sg01_0003"></a>

## Function<a name="section4195542395259"></a>

This API is used to query security groups using search criteria and to display the security groups in a list.

## URI<a name="section5844660495259"></a>

GET /v1/\{project\_id\}/security-groups

Example:

```
GET https://{Endpoint}/v1/{project_id}/security-groups?limit=10&marker=4779ab1c-7c1a-44b1-a02e-93dfc361b32d&vpc_id=3ec3b33f-ac1c-4630-ad1c-7dba1ed79d85
```

[Table 1](#table1939240195259)  describes the parameters.

**Table  1**  Parameter description

<a name="table1939240195259"></a>
<table><thead align="left"><tr id="row1961474195259"><th class="cellrowborder" valign="top" width="17.349999999999998%" id="mcps1.2.5.1.1"><p id="p1035476495259"><a name="p1035476495259"></a><a name="p1035476495259"></a>Name</p>
</th>
<th class="cellrowborder" valign="top" width="22.21%" id="mcps1.2.5.1.2"><p id="p1553041195259"><a name="p1553041195259"></a><a name="p1553041195259"></a>Mandatory</p>
</th>
<th class="cellrowborder" valign="top" width="29.830000000000002%" id="mcps1.2.5.1.3"><p id="p112673695259"><a name="p112673695259"></a><a name="p112673695259"></a>Type</p>
</th>
<th class="cellrowborder" valign="top" width="30.61%" id="mcps1.2.5.1.4"><p id="p2600047695259"><a name="p2600047695259"></a><a name="p2600047695259"></a>Description</p>
</th>
</tr>
</thead>
<tbody><tr id="row1253681595259"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p2796266695259"><a name="p2796266695259"></a><a name="p2796266695259"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.21%" headers="mcps1.2.5.1.2 "><p id="p3612906795259"><a name="p3612906795259"></a><a name="p3612906795259"></a>Yes</p>
</td>
<td class="cellrowborder" valign="top" width="29.830000000000002%" headers="mcps1.2.5.1.3 "><p id="p2573237195259"><a name="p2573237195259"></a><a name="p2573237195259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>Specifies the project ID. </p>
</td>
</tr>
<tr id="row4225519995259"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p137426195259"><a name="p137426195259"></a><a name="p137426195259"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="22.21%" headers="mcps1.2.5.1.2 "><p id="p3252720195259"><a name="p3252720195259"></a><a name="p3252720195259"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="29.830000000000002%" headers="mcps1.2.5.1.3 "><p id="p308224595259"><a name="p308224595259"></a><a name="p308224595259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><p id="p3140128095259"><a name="p3140128095259"></a><a name="p3140128095259"></a>Specifies the start resource ID of pagination query. If the parameter is left blank, only resources on the first page are queried.</p>
</td>
</tr>
<tr id="row5868376895259"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p6257361795259"><a name="p6257361795259"></a><a name="p6257361795259"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="22.21%" headers="mcps1.2.5.1.2 "><p id="p439086695259"><a name="p439086695259"></a><a name="p439086695259"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="29.830000000000002%" headers="mcps1.2.5.1.3 "><p id="p3106751395259"><a name="p3106751395259"></a><a name="p3106751395259"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><a name="ul9752142515014"></a><a name="ul9752142515014"></a><ul id="ul9752142515014"><li>Specifies the number of records returned on each page.</li><li>The value ranges from 0 to intmax.</li></ul>
</td>
</tr>
<tr id="row2580668495259"><td class="cellrowborder" valign="top" width="17.349999999999998%" headers="mcps1.2.5.1.1 "><p id="p2103752995259"><a name="p2103752995259"></a><a name="p2103752995259"></a>vpc_id</p>
</td>
<td class="cellrowborder" valign="top" width="22.21%" headers="mcps1.2.5.1.2 "><p id="p5853666895259"><a name="p5853666895259"></a><a name="p5853666895259"></a>No</p>
</td>
<td class="cellrowborder" valign="top" width="29.830000000000002%" headers="mcps1.2.5.1.3 "><p id="p6330151095259"><a name="p6330151095259"></a><a name="p6330151095259"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="30.61%" headers="mcps1.2.5.1.4 "><p id="p3783295295259"><a name="p3783295295259"></a><a name="p3783295295259"></a>Specifies that the VPC ID is used as the filtering condition.</p>
</td>
</tr>
</tbody>
</table>

## Request Message<a name="section3936161695259"></a>

-   Request parameter

    None

-   Example request

    ```
    GET https://{Endpoint}/v1/{project_id}/security-groups
    ```


## Response Message<a name="section3532656695259"></a>

-   Response parameter

    **Table  2**  Response parameter

    <a name="table3248515795259"></a>
    <table><thead align="left"><tr id="row1680595259"><th class="cellrowborder" valign="top" width="23.26%" id="mcps1.2.4.1.1"><p id="p1326742895259"><a name="p1326742895259"></a><a name="p1326742895259"></a>Name</p>
    </th>
    <th class="cellrowborder" valign="top" width="22.09%" id="mcps1.2.4.1.2"><p id="p1250466195259"><a name="p1250466195259"></a><a name="p1250466195259"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="54.65%" id="mcps1.2.4.1.3"><p id="p2003783295259"><a name="p2003783295259"></a><a name="p2003783295259"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row4409981195259"><td class="cellrowborder" valign="top" width="23.26%" headers="mcps1.2.4.1.1 "><p id="p1222895259"><a name="p1222895259"></a><a name="p1222895259"></a>security_groups</p>
    </td>
    <td class="cellrowborder" valign="top" width="22.09%" headers="mcps1.2.4.1.2 "><p id="p2797014095259"><a name="p2797014095259"></a><a name="p2797014095259"></a>Array of <a href="#table333218689520">security_group</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="54.65%" headers="mcps1.2.4.1.3 "><p id="p3551241495259"><a name="p3551241495259"></a><a name="p3551241495259"></a>Specifies the security group objects. For details, see <a href="#table333218689520">Table 3</a>.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **Table  3**  Description of  **security\_group**  fields

    <a name="table333218689520"></a>
    <table><thead align="left"><tr id="vpc_sg01_0001_row158029169489"><th class="cellrowborder" valign="top" width="34.52%" id="mcps1.2.4.1.1"><p id="vpc_sg01_0001_p581966039489"><a name="vpc_sg01_0001_p581966039489"></a><a name="vpc_sg01_0001_p581966039489"></a>Name</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.45%" id="mcps1.2.4.1.2"><p id="vpc_sg01_0001_p166624639489"><a name="vpc_sg01_0001_p166624639489"></a><a name="vpc_sg01_0001_p166624639489"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="44.03%" id="mcps1.2.4.1.3"><p id="vpc_sg01_0001_p278965559489"><a name="vpc_sg01_0001_p278965559489"></a><a name="vpc_sg01_0001_p278965559489"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="vpc_sg01_0001_row643785269489"><td class="cellrowborder" valign="top" width="34.52%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p329359299489"><a name="vpc_sg01_0001_p329359299489"></a><a name="vpc_sg01_0001_p329359299489"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p230963549489"><a name="vpc_sg01_0001_p230963549489"></a><a name="vpc_sg01_0001_p230963549489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.03%" headers="mcps1.2.4.1.3 "><p id="vpc_sg01_0001_p410063869489"><a name="vpc_sg01_0001_p410063869489"></a><a name="vpc_sg01_0001_p410063869489"></a>Specifies the security group name.</p>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row32100149489"><td class="cellrowborder" valign="top" width="34.52%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p522665169489"><a name="vpc_sg01_0001_p522665169489"></a><a name="vpc_sg01_0001_p522665169489"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p513285489489"><a name="vpc_sg01_0001_p513285489489"></a><a name="vpc_sg01_0001_p513285489489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.03%" headers="mcps1.2.4.1.3 "><p id="vpc_sg01_0001_p290727679489"><a name="vpc_sg01_0001_p290727679489"></a><a name="vpc_sg01_0001_p290727679489"></a>Provides supplementary information about the security group.</p>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row639972559489"><td class="cellrowborder" valign="top" width="34.52%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p634276169489"><a name="vpc_sg01_0001_p634276169489"></a><a name="vpc_sg01_0001_p634276169489"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p114487449489"><a name="vpc_sg01_0001_p114487449489"></a><a name="vpc_sg01_0001_p114487449489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.03%" headers="mcps1.2.4.1.3 "><p id="vpc_sg01_0001_p259109349489"><a name="vpc_sg01_0001_p259109349489"></a><a name="vpc_sg01_0001_p259109349489"></a>Specifies the security group ID, which uniquely identifies the security group.</p>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row422544629489"><td class="cellrowborder" valign="top" width="34.52%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p590727719489"><a name="vpc_sg01_0001_p590727719489"></a><a name="vpc_sg01_0001_p590727719489"></a>vpc_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p10272179489"><a name="vpc_sg01_0001_p10272179489"></a><a name="vpc_sg01_0001_p10272179489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.03%" headers="mcps1.2.4.1.3 "><p id="vpc_sg01_0001_p303149719489"><a name="vpc_sg01_0001_p303149719489"></a><a name="vpc_sg01_0001_p303149719489"></a>Specifies the resource ID of the VPC to which the security group belongs.</p>
    <div class="note" id="vpc_sg01_0001_note1071412434342"><a name="vpc_sg01_0001_note1071412434342"></a><a name="vpc_sg01_0001_note1071412434342"></a><span class="notetitle"> NOTE: </span><div class="notebody"><p id="vpc_sg01_0001_p137151443133411"><a name="vpc_sg01_0001_p137151443133411"></a><a name="vpc_sg01_0001_p137151443133411"></a>This parameter has been discarded, it is not recommended to use it.</p>
    </div></div>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row30397199489"><td class="cellrowborder" valign="top" width="34.52%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p252491199489"><a name="vpc_sg01_0001_p252491199489"></a><a name="vpc_sg01_0001_p252491199489"></a>security_group_rules</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.45%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p193798449489"><a name="vpc_sg01_0001_p193798449489"></a><a name="vpc_sg01_0001_p193798449489"></a>Array of <a href="creating-a-security-group.md#table210704979489">security_group_rule</a> objects</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.03%" headers="mcps1.2.4.1.3 "><p id="vpc_sg01_0001_p643841019489"><a name="vpc_sg01_0001_p643841019489"></a><a name="vpc_sg01_0001_p643841019489"></a>Specifies the default security group rule, which ensures that resources in the security group can communicate with one another.</p>
    </td>
    </tr>
    </tbody>
    </table>

    **Table  4** **security\_group\_rule**  objects

    <a name="table488727239520"></a>
    <table><thead align="left"><tr id="vpc_sg01_0001_row611024789489"><th class="cellrowborder" valign="top" width="34.143414341434145%" id="mcps1.2.4.1.1"><p id="vpc_sg01_0001_p98931099489"><a name="vpc_sg01_0001_p98931099489"></a><a name="vpc_sg01_0001_p98931099489"></a>Name</p>
    </th>
    <th class="cellrowborder" valign="top" width="20.732073207320735%" id="mcps1.2.4.1.2"><p id="vpc_sg01_0001_p368367439489"><a name="vpc_sg01_0001_p368367439489"></a><a name="vpc_sg01_0001_p368367439489"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="45.124512451245124%" id="mcps1.2.4.1.3"><p id="vpc_sg01_0001_p23523719489"><a name="vpc_sg01_0001_p23523719489"></a><a name="vpc_sg01_0001_p23523719489"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="vpc_sg01_0001_row397690789489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p656951529489"><a name="vpc_sg01_0001_p656951529489"></a><a name="vpc_sg01_0001_p656951529489"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p307102169489"><a name="vpc_sg01_0001_p307102169489"></a><a name="vpc_sg01_0001_p307102169489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><p id="vpc_sg01_0001_p216633359489"><a name="vpc_sg01_0001_p216633359489"></a><a name="vpc_sg01_0001_p216633359489"></a>Specifies the security group rule ID, which uniquely identifies the security group rule.</p>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row2447898388"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p432391116381"><a name="vpc_sg01_0001_p432391116381"></a><a name="vpc_sg01_0001_p432391116381"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p20328111163813"><a name="vpc_sg01_0001_p20328111163813"></a><a name="vpc_sg01_0001_p20328111163813"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><a name="vpc_sg01_0001_ul12329121935111"></a><a name="vpc_sg01_0001_ul12329121935111"></a><ul id="vpc_sg01_0001_ul12329121935111"><li>Provides supplementary information about the security group rule.</li><li>The value is a string of no more than 255 characters that can contain letters and digits.</li></ul>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row320377939489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p620577269489"><a name="vpc_sg01_0001_p620577269489"></a><a name="vpc_sg01_0001_p620577269489"></a>security_group_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p644725909489"><a name="vpc_sg01_0001_p644725909489"></a><a name="vpc_sg01_0001_p644725909489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><p id="vpc_sg01_0001_p260700169489"><a name="vpc_sg01_0001_p260700169489"></a><a name="vpc_sg01_0001_p260700169489"></a>Specifies the security group rule ID, which uniquely identifies the security group rule.</p>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row602307149489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p184092199489"><a name="vpc_sg01_0001_p184092199489"></a><a name="vpc_sg01_0001_p184092199489"></a>direction</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p499849219489"><a name="vpc_sg01_0001_p499849219489"></a><a name="vpc_sg01_0001_p499849219489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><a name="vpc_sg01_0001_ul8415142317513"></a><a name="vpc_sg01_0001_ul8415142317513"></a><ul id="vpc_sg01_0001_ul8415142317513"><li>Specifies the direction of access control.</li><li>Possible values are as follows:<a name="vpc_sg01_0001_ul6968104419355"></a><a name="vpc_sg01_0001_ul6968104419355"></a><ul id="vpc_sg01_0001_ul6968104419355"><li><strong id="vpc_sg01_0001_b96381611133314"><a name="vpc_sg01_0001_b96381611133314"></a><a name="vpc_sg01_0001_b96381611133314"></a>egress</strong></li><li><strong id="vpc_sg01_0001_b9979172133411"><a name="vpc_sg01_0001_b9979172133411"></a><a name="vpc_sg01_0001_b9979172133411"></a>ingress</strong></li></ul>
    </li></ul>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row53906049489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p460392719489"><a name="vpc_sg01_0001_p460392719489"></a><a name="vpc_sg01_0001_p460392719489"></a>ethertype</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p248464689489"><a name="vpc_sg01_0001_p248464689489"></a><a name="vpc_sg01_0001_p248464689489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><a name="vpc_sg01_0001_ul78261926205119"></a><a name="vpc_sg01_0001_ul78261926205119"></a><ul id="vpc_sg01_0001_ul78261926205119"><li>Specifies the IP protocol version.</li><li>The value can be <strong>IPv4</strong> or <strong>IPv6</strong>.</li></ul>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row619098859489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p520137079489"><a name="vpc_sg01_0001_p520137079489"></a><a name="vpc_sg01_0001_p520137079489"></a>protocol</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p17867349489"><a name="vpc_sg01_0001_p17867349489"></a><a name="vpc_sg01_0001_p17867349489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><a name="vpc_sg01_0001_ul585593011517"></a><a name="vpc_sg01_0001_ul585593011517"></a><ul id="vpc_sg01_0001_ul585593011517"><li>Specifies the protocol type.</li><li>The value can be <strong id="vpc_sg01_0001_b1459493374214"><a name="vpc_sg01_0001_b1459493374214"></a><a name="vpc_sg01_0001_b1459493374214"></a>icmp</strong>, <strong id="vpc_sg01_0001_b115948336427"><a name="vpc_sg01_0001_b115948336427"></a><a name="vpc_sg01_0001_b115948336427"></a>tcp</strong>, or <strong id="vpc_sg01_0001_b659723354216"><a name="vpc_sg01_0001_b659723354216"></a><a name="vpc_sg01_0001_b659723354216"></a>udp</strong>.</li><li>If the parameter is left blank, all protocols are supported.</li></ul>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row29885099489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p424368709489"><a name="vpc_sg01_0001_p424368709489"></a><a name="vpc_sg01_0001_p424368709489"></a>port_range_min</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p167549899489"><a name="vpc_sg01_0001_p167549899489"></a><a name="vpc_sg01_0001_p167549899489"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><a name="vpc_sg01_0001_ul1445493595119"></a><a name="vpc_sg01_0001_ul1445493595119"></a><ul id="vpc_sg01_0001_ul1445493595119"><li>Specifies the start port number.</li><li>The value ranges from 1 to 65535.</li><li>The value cannot be greater than the <strong id="vpc_sg01_0001_b842352706195750"><a name="vpc_sg01_0001_b842352706195750"></a><a name="vpc_sg01_0001_b842352706195750"></a>port_range_max</strong> value. An empty value indicates all ports. If the protocol is <strong id="vpc_sg01_0001_b842352706195910"><a name="vpc_sg01_0001_b842352706195910"></a><a name="vpc_sg01_0001_b842352706195910"></a>icmp</strong>, the value range is shown in <a href="icmp-port-range-relationship-table.md">ICMP-Port Range Relationship Table</a>.</li></ul>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row330228649489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p239666849489"><a name="vpc_sg01_0001_p239666849489"></a><a name="vpc_sg01_0001_p239666849489"></a>port_range_max</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p641378179489"><a name="vpc_sg01_0001_p641378179489"></a><a name="vpc_sg01_0001_p641378179489"></a>Integer</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><a name="vpc_sg01_0001_ul23372407514"></a><a name="vpc_sg01_0001_ul23372407514"></a><ul id="vpc_sg01_0001_ul23372407514"><li>Specifies the end port number.</li><li>The value ranges from 1 to 65535.</li><li>If the protocol is not <strong id="vpc_sg01_0001_b842352706195730"><a name="vpc_sg01_0001_b842352706195730"></a><a name="vpc_sg01_0001_b842352706195730"></a>icmp</strong>, the value cannot be smaller than the <strong id="vpc_sg01_0001_b33723164"><a name="vpc_sg01_0001_b33723164"></a><a name="vpc_sg01_0001_b33723164"></a>port_range_min</strong> value. An empty value indicates all ports. If the protocol is <strong id="vpc_sg01_0001_b1736655103"><a name="vpc_sg01_0001_b1736655103"></a><a name="vpc_sg01_0001_b1736655103"></a>icmp</strong>, the value range is shown in <a href="icmp-port-range-relationship-table.md">ICMP-Port Range Relationship Table</a>.</li></ul>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row1745649489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p144166029489"><a name="vpc_sg01_0001_p144166029489"></a><a name="vpc_sg01_0001_p144166029489"></a>remote_ip_prefix</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p139601239489"><a name="vpc_sg01_0001_p139601239489"></a><a name="vpc_sg01_0001_p139601239489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><a name="vpc_sg01_0001_ul42481344125119"></a><a name="vpc_sg01_0001_ul42481344125119"></a><ul id="vpc_sg01_0001_ul42481344125119"><li>Specifies the remote IP address. If the access control direction is set to <strong>egress</strong>, the parameter specifies the source IP address. If the access control direction is set to <strong>ingress</strong>, the parameter specifies the destination IP address.</li><li>The value can be in the CIDR format or IP addresses.</li><li>The parameter is exclusive with parameter <strong>remote_group_id</strong>.</li></ul>
    </td>
    </tr>
    <tr id="vpc_sg01_0001_row436879079489"><td class="cellrowborder" valign="top" width="34.143414341434145%" headers="mcps1.2.4.1.1 "><p id="vpc_sg01_0001_p420105089489"><a name="vpc_sg01_0001_p420105089489"></a><a name="vpc_sg01_0001_p420105089489"></a>remote_group_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.732073207320735%" headers="mcps1.2.4.1.2 "><p id="vpc_sg01_0001_p465213149489"><a name="vpc_sg01_0001_p465213149489"></a><a name="vpc_sg01_0001_p465213149489"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="45.124512451245124%" headers="mcps1.2.4.1.3 "><a name="vpc_sg01_0001_ul12672447145118"></a><a name="vpc_sg01_0001_ul12672447145118"></a><ul id="vpc_sg01_0001_ul12672447145118"><li>Specifies the ID of the peer security group.</li><li>The value is exclusive with parameter <strong>remote_ip_prefix</strong>.</li></ul>
    </td>
    </tr>
    </tbody>
    </table>


-   Example response

    ```
    {
        "security_groups": [
            {
                "id": "16b6e77a-08fa-42c7-aa8b-106c048884e6", 
                "name": "qq", 
                "description": "qq", 
                "vpc_id": "3ec3b33f-ac1c-4630-ad1c-7dba1ed79d85", 
               
                "security_group_rules": [
                    {
                        "direction": "egress", 
                        "ethertype": "IPv4", 
                        "id": "369e6499-b2cb-4126-972a-97e589692c62", 
                        "description": "",
                        "security_group_id": "16b6e77a-08fa-42c7-aa8b-106c048884e6"
                    }, 
                    {
                        "direction": "ingress", 
                        "ethertype": "IPv4", 
                        "id": "0222556c-6556-40ad-8aac-9fd5d3c06171", 
                        "description": "",
                        "remote_group_id": "16b6e77a-08fa-42c7-aa8b-106c048884e6", 
                        "security_group_id": "16b6e77a-08fa-42c7-aa8b-106c048884e6"
                    }
                ]
            }, 
            {
                "id": "9c0f56be-a9ac-438c-8c57-fce62de19419", 
                "name": "default", 
                "description": "qq", 
                "vpc_id": "13551d6b-755d-4757-b956-536f674975c0", 
               
                "security_group_rules": [
                    {
                        "direction": "egress", 
                        "ethertype": "IPv4", 
                        "id": "95479e0a-e312-4844-b53d-a5e4541b783f", 
                        "description": "",
                        "security_group_id": "9c0f56be-a9ac-438c-8c57-fce62de19419"
                    }, 
                    {
                        "direction": "ingress", 
                        "ethertype": "IPv4", 
                        "id": "0c4a2336-b036-4fa2-bc3c-1a291ed4c431",
                        "description": "", 
                        "remote_group_id": "9c0f56be-a9ac-438c-8c57-fce62de19419", 
                        "security_group_id": "9c0f56be-a9ac-438c-8c57-fce62de19419"
                    }
                ]
            }
        ]
    }
    ```


## Status Code<a name="section31981619"></a>

See  [Status Codes](status-codes.md).

## Error Code<a name="section85821649202813"></a>

See  [Error Codes](error-codes.md).

