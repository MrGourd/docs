# Deleting a User from a User Group<a name="en-us_topic_0057845601"></a>

## Function Description<a name="section495175389414"></a>

This interface is used to delete a user from a user group.

## URI<a name="section3019338085013"></a>

-   URI format

    DELETE /v3/groups/\{group\_id\}/users/\{user\_id\}

-   URI parameter description

    <a name="en-us_topic_0032920307_table36168141"></a>
    <table><thead align="left"><tr id="en-us_topic_0032920307_row15662289"><th class="cellrowborder" valign="top" width="19.36%" id="mcps1.1.5.1.1"><p id="en-us_topic_0032920307_p60685926"><a name="en-us_topic_0032920307_p60685926"></a><a name="en-us_topic_0032920307_p60685926"></a><strong id="b842352706111527"><a name="b842352706111527"></a><a name="b842352706111527"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="19.24%" id="mcps1.1.5.1.2"><p id="en-us_topic_0032920307_p16612996"><a name="en-us_topic_0032920307_p16612996"></a><a name="en-us_topic_0032920307_p16612996"></a><strong id="a105e6ed8c3de4c5a9dde97ae5a71071e_1"><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_1"></a><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_1"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="17.98%" id="mcps1.1.5.1.3"><p id="en-us_topic_0032920307_p3475410"><a name="en-us_topic_0032920307_p3475410"></a><a name="en-us_topic_0032920307_p3475410"></a><strong id="b842352706143526_1"><a name="b842352706143526_1"></a><a name="b842352706143526_1"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="43.419999999999995%" id="mcps1.1.5.1.4"><p id="en-us_topic_0032920307_p13072760"><a name="en-us_topic_0032920307_p13072760"></a><a name="en-us_topic_0032920307_p13072760"></a><strong id="b20601766145329"><a name="b20601766145329"></a><a name="b20601766145329"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="en-us_topic_0032920307_row52260639"><td class="cellrowborder" valign="top" width="19.36%" headers="mcps1.1.5.1.1 "><p id="en-us_topic_0032920307_p5253358"><a name="en-us_topic_0032920307_p5253358"></a><a name="en-us_topic_0032920307_p5253358"></a>group_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.1.5.1.2 "><p id="en-us_topic_0032920307_p22868878"><a name="en-us_topic_0032920307_p22868878"></a><a name="en-us_topic_0032920307_p22868878"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.98%" headers="mcps1.1.5.1.3 "><p id="en-us_topic_0032920307_p40439847"><a name="en-us_topic_0032920307_p40439847"></a><a name="en-us_topic_0032920307_p40439847"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.5.1.4 "><p id="en-us_topic_0032920307_p54402144"><a name="en-us_topic_0032920307_p54402144"></a><a name="en-us_topic_0032920307_p54402144"></a>ID of a user group.</p>
    </td>
    </tr>
    <tr id="row980208103522"><td class="cellrowborder" valign="top" width="19.36%" headers="mcps1.1.5.1.1 "><p id="p8821877103522"><a name="p8821877103522"></a><a name="p8821877103522"></a>user_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.24%" headers="mcps1.1.5.1.2 "><p id="p43483414103522"><a name="p43483414103522"></a><a name="p43483414103522"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.98%" headers="mcps1.1.5.1.3 "><p id="p32495677103522"><a name="p32495677103522"></a><a name="p32495677103522"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.5.1.4 "><p id="p14904143103522"><a name="p14904143103522"></a><a name="p14904143103522"></a>ID of a user.</p>
    </td>
    </tr>
    </tbody>
    </table>


## Request<a name="section1437107585444"></a>

-   Request header parameter description

    <a name="en-us_topic_0032920307_table21736211"></a>
    <table><thead align="left"><tr id="en-us_topic_0032920307_row48433347"><th class="cellrowborder" valign="top" width="19.49%" id="mcps1.1.5.1.1"><p id="en-us_topic_0032920307_p30787047"><a name="en-us_topic_0032920307_p30787047"></a><a name="en-us_topic_0032920307_p30787047"></a><strong id="a173ae121cc9e48328ca613e72f2a1504"><a name="a173ae121cc9e48328ca613e72f2a1504"></a><a name="a173ae121cc9e48328ca613e72f2a1504"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="18.86%" id="mcps1.1.5.1.2"><p id="en-us_topic_0032920307_p10722842"><a name="en-us_topic_0032920307_p10722842"></a><a name="en-us_topic_0032920307_p10722842"></a><strong id="a105e6ed8c3de4c5a9dde97ae5a71071e_3"><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_3"></a><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_3"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="17.44%" id="mcps1.1.5.1.3"><p id="en-us_topic_0032920307_p63243911"><a name="en-us_topic_0032920307_p63243911"></a><a name="en-us_topic_0032920307_p63243911"></a><strong id="b842352706143526_3"><a name="b842352706143526_3"></a><a name="b842352706143526_3"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="44.21%" id="mcps1.1.5.1.4"><p id="en-us_topic_0032920307_p22483156"><a name="en-us_topic_0032920307_p22483156"></a><a name="en-us_topic_0032920307_p22483156"></a><strong id="b1118670614468"><a name="b1118670614468"></a><a name="b1118670614468"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="en-us_topic_0032920307_row9196329"><td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.1 "><p id="en-us_topic_0032920307_p6705199"><a name="en-us_topic_0032920307_p6705199"></a><a name="en-us_topic_0032920307_p6705199"></a>Content-Type</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.1.5.1.2 "><p id="en-us_topic_0032920307_p6250253"><a name="en-us_topic_0032920307_p6250253"></a><a name="en-us_topic_0032920307_p6250253"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.5.1.3 "><p id="en-us_topic_0032920307_p36508524"><a name="en-us_topic_0032920307_p36508524"></a><a name="en-us_topic_0032920307_p36508524"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.21%" headers="mcps1.1.5.1.4 "><p id="en-us_topic_0032920307_p4400500"><a name="en-us_topic_0032920307_p4400500"></a><a name="en-us_topic_0032920307_p4400500"></a>Fill <strong id="b842352706161331"><a name="b842352706161331"></a><a name="b842352706161331"></a>application/json;charset=utf8</strong> in this field.</p>
    </td>
    </tr>
    <tr id="en-us_topic_0032920307_row39604502"><td class="cellrowborder" valign="top" width="19.49%" headers="mcps1.1.5.1.1 "><p id="en-us_topic_0032920307_p53848109"><a name="en-us_topic_0032920307_p53848109"></a><a name="en-us_topic_0032920307_p53848109"></a>X-Auth-Token</p>
    </td>
    <td class="cellrowborder" valign="top" width="18.86%" headers="mcps1.1.5.1.2 "><p id="en-us_topic_0032920307_p66729601"><a name="en-us_topic_0032920307_p66729601"></a><a name="en-us_topic_0032920307_p66729601"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.44%" headers="mcps1.1.5.1.3 "><p id="en-us_topic_0032920307_p36388601"><a name="en-us_topic_0032920307_p36388601"></a><a name="en-us_topic_0032920307_p36388601"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="44.21%" headers="mcps1.1.5.1.4 "><p id="p307328551134"><a name="p307328551134"></a><a name="p307328551134"></a>Authenticated token with the <strong id="b750798910387"><a name="b750798910387"></a><a name="b750798910387"></a>Security Administrator</strong> permission.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Sample request

    ```
    curl -i -k -H 'Accept:application/json' -H 'Content-Type:application/json;charset=utf8' -H "X-Auth-Token:$token" -X DELETE https://172.30.48.86:31943/v3/groups/00007111583e457389b0d4252643181b/users/edb66d2b656c43d0b67fb143d670bb3a
    ```


## Response<a name="section728317461105"></a>

No response body.

## Status Codes<a name="section5556784894735"></a>

<a name="en-us_topic_0032920307_table25927028"></a>
<table><thead align="left"><tr id="en-us_topic_0032920307_row10578662"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="en-us_topic_0032920307_p51565323"><a name="en-us_topic_0032920307_p51565323"></a><a name="en-us_topic_0032920307_p51565323"></a><strong id="b842352706183230"><a name="b842352706183230"></a><a name="b842352706183230"></a>Status Code</strong></p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="en-us_topic_0032920307_p16041657"><a name="en-us_topic_0032920307_p16041657"></a><a name="en-us_topic_0032920307_p16041657"></a><strong id="b3318686714468"><a name="b3318686714468"></a><a name="b3318686714468"></a>Description</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="en-us_topic_0032920307_row24305815"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0032920307_p22613965"><a name="en-us_topic_0032920307_p22613965"></a><a name="en-us_topic_0032920307_p22613965"></a>204</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="en-us_topic_0032920307_p19791876"><a name="en-us_topic_0032920307_p19791876"></a><a name="en-us_topic_0032920307_p19791876"></a>The request is successful.</p>
</td>
</tr>
<tr id="en-us_topic_0032920307_row43909159"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0032920307_p66980994"><a name="en-us_topic_0032920307_p66980994"></a><a name="en-us_topic_0032920307_p66980994"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p429015435323"><a name="p429015435323"></a><a name="p429015435323"></a>The server failed to process the request.</p>
</td>
</tr>
<tr id="row460808479497"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p120744399497"><a name="p120744399497"></a><a name="p120744399497"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p385055099497"><a name="p385055099497"></a><a name="p385055099497"></a>You must enter a username and password to access the requested page.</p>
</td>
</tr>
<tr id="en-us_topic_0032920307_row41000636"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0032920307_p32717189"><a name="en-us_topic_0032920307_p32717189"></a><a name="en-us_topic_0032920307_p32717189"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="en-us_topic_0032920307_p32846614"><a name="en-us_topic_0032920307_p32846614"></a><a name="en-us_topic_0032920307_p32846614"></a>You are forbidden to access the requested page.</p>
</td>
</tr>
<tr id="row2569718985351"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p2994811485351"><a name="p2994811485351"></a><a name="p2994811485351"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p987817085351"><a name="p987817085351"></a><a name="p987817085351"></a>The server could not find the requested page.</p>
</td>
</tr>
</tbody>
</table>

