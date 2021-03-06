# Querying Tags of a Backup Policy<a name="EN-US_TOPIC_0067142131"></a>

## Function<a name="section63962185"></a>

This interface is used to query the tags of a specific backup policy.

## URI<a name="section38788755"></a>

-   URI format

    GET /v2/\{project\_id\}/backuppolicy/\{policy\_id\}/tags

-   Parameter description

    <a name="table60344938"></a>
    <table><thead align="left"><tr id="row59011071"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.1"><p id="p15167431"><a name="p15167431"></a><a name="p15167431"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.2"><p id="p20602375"><a name="p20602375"></a><a name="p20602375"></a>Mandatory</p>
    </th>
    <th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.1.4.1.3"><p id="p58179688"><a name="p58179688"></a><a name="p58179688"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row14934289"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p1717931"><a name="p1717931"></a><a name="p1717931"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p4934750"><a name="p4934750"></a><a name="p4934750"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p64170449"><a name="p64170449"></a><a name="p64170449"></a>Project ID</p>
    </td>
    </tr>
    <tr id="row49177768142544"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.1 "><p id="p23976272142544"><a name="p23976272142544"></a><a name="p23976272142544"></a>policy_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.2 "><p id="p63029893142544"><a name="p63029893142544"></a><a name="p63029893142544"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.1.4.1.3 "><p id="p5147694142544"><a name="p5147694142544"></a><a name="p5147694142544"></a>Backup policy ID</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Example request

    ```
    GET /v2/{project_id}/backuppolicy/{policy_id}/tags
    ```


## Request<a name="section13554483"></a>

None

## Response<a name="section54881489"></a>

-   Parameter description

    <a name="table65890561182249"></a>
    <table><thead align="left"><tr id="row28557550182249"><th class="cellrowborder" valign="top" width="25.840000000000003%" id="mcps1.1.4.1.1"><p id="p1431817452527"><a name="p1431817452527"></a><a name="p1431817452527"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="16.74%" id="mcps1.1.4.1.2"><p id="p14225104112"><a name="p14225104112"></a><a name="p14225104112"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.42%" id="mcps1.1.4.1.3"><p id="p29622330"><a name="p29622330"></a><a name="p29622330"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59988132182249"><td class="cellrowborder" valign="top" width="25.840000000000003%" headers="mcps1.1.4.1.1 "><p id="p27200506182249"><a name="p27200506182249"></a><a name="p27200506182249"></a>tags</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.74%" headers="mcps1.1.4.1.2 "><p id="p20056653182249"><a name="p20056653182249"></a><a name="p20056653182249"></a>list&lt;dict&gt;</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42%" headers="mcps1.1.4.1.3 "><p id="p13976217182249"><a name="p13976217182249"></a><a name="p13976217182249"></a>List of tag details</p>
    </td>
    </tr>
    <tr id="row58677097182249"><td class="cellrowborder" valign="top" width="25.840000000000003%" headers="mcps1.1.4.1.1 "><p id="p55224391182249"><a name="p55224391182249"></a><a name="p55224391182249"></a>key</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.74%" headers="mcps1.1.4.1.2 "><p id="p6473140182249"><a name="p6473140182249"></a><a name="p6473140182249"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42%" headers="mcps1.1.4.1.3 "><p id="p54562323182249"><a name="p54562323182249"></a><a name="p54562323182249"></a>Tag key</p>
    </td>
    </tr>
    <tr id="row21298866182249"><td class="cellrowborder" valign="top" width="25.840000000000003%" headers="mcps1.1.4.1.1 "><p id="p47486561182249"><a name="p47486561182249"></a><a name="p47486561182249"></a>value</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.74%" headers="mcps1.1.4.1.2 "><p id="p39982301182249"><a name="p39982301182249"></a><a name="p39982301182249"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42%" headers="mcps1.1.4.1.3 "><p id="p17340921182249"><a name="p17340921182249"></a><a name="p17340921182249"></a>Tag value</p>
    </td>
    </tr>
    <tr id="row21850568182249"><td class="cellrowborder" valign="top" width="25.840000000000003%" headers="mcps1.1.4.1.1 "><p id="p25065570182249"><a name="p25065570182249"></a><a name="p25065570182249"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.74%" headers="mcps1.1.4.1.2 "><p id="p38492801182249"><a name="p38492801182249"></a><a name="p38492801182249"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42%" headers="mcps1.1.4.1.3 "><p id="p30909140182249"><a name="p30909140182249"></a><a name="p30909140182249"></a>Error message returned after an error occurs</p>
    </td>
    </tr>
    <tr id="row9746812182249"><td class="cellrowborder" valign="top" width="25.840000000000003%" headers="mcps1.1.4.1.1 "><p id="p51294316182249"><a name="p51294316182249"></a><a name="p51294316182249"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.74%" headers="mcps1.1.4.1.2 "><p id="p58164833182249"><a name="p58164833182249"></a><a name="p58164833182249"></a>string</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.42%" headers="mcps1.1.4.1.3 "><p id="p13730998182249"><a name="p13730998182249"></a><a name="p13730998182249"></a>Error code returned after an error occurs</p>
    <p id="p56470119182249"><a name="p56470119182249"></a><a name="p56470119182249"></a>For details about error codes, see <a href="error-codes.md">Error Codes</a>.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Example response

    ```
    {
      "tags": [
        {
          "key": "RUNNING",
          "value":"0781095c-b8ab-4ce5-99f3-4c5f6ff75319"
        },
        {
          "key": "WAITING",
          "values":"2016-12-03T06:24:34.467"
        }
      ]
    }
    ```

    or

    ```
    {
        "error": {
            "message": "XXXX",
            "code": "XXX"
        }
    }
    ```


## Status Codes<a name="section24171358"></a>

-   Normal

    200

-   Abnormal

    <a name="table51230787"></a>
    <table><thead align="left"><tr id="row60503138"><th class="cellrowborder" valign="top" width="43.419999999999995%" id="mcps1.1.3.1.1"><p id="p1807185"><a name="p1807185"></a><a name="p1807185"></a>Status Code</p>
    </th>
    <th class="cellrowborder" valign="top" width="56.58%" id="mcps1.1.3.1.2"><p id="p12164329"><a name="p12164329"></a><a name="p12164329"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row45786577"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p17725233"><a name="p17725233"></a><a name="p17725233"></a>400 Bad Request</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p26457778"><a name="p26457778"></a><a name="p26457778"></a>The server failed to process the request.</p>
    </td>
    </tr>
    <tr id="row36793414"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p27476571"><a name="p27476571"></a><a name="p27476571"></a>401 Unauthorized</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p11009764"><a name="p11009764"></a><a name="p11009764"></a>You must enter the username and password to access the requested page.</p>
    </td>
    </tr>
    <tr id="row31979016"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p40163483"><a name="p40163483"></a><a name="p40163483"></a>403 Forbidden</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p32016662"><a name="p32016662"></a><a name="p32016662"></a>You are forbidden to access the requested page.</p>
    </td>
    </tr>
    <tr id="row4499052116376"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p2035357816376"><a name="p2035357816376"></a><a name="p2035357816376"></a>404 Not Found</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p3802708716376"><a name="p3802708716376"></a><a name="p3802708716376"></a>The server could not find the requested page.</p>
    </td>
    </tr>
    <tr id="row8462523163725"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p14375766163725"><a name="p14375766163725"></a><a name="p14375766163725"></a>405 Method Not Allowed</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p23586373163725"><a name="p23586373163725"></a><a name="p23586373163725"></a>You are not allowed to use the method specified in the request.</p>
    </td>
    </tr>
    <tr id="row60343628163758"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p55995701163758"><a name="p55995701163758"></a><a name="p55995701163758"></a>406 Not Acceptable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p39357967163758"><a name="p39357967163758"></a><a name="p39357967163758"></a>The response generated by the server could not be accepted by the client.</p>
    </td>
    </tr>
    <tr id="row32079544163754"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p48306260163754"><a name="p48306260163754"></a><a name="p48306260163754"></a>407 Proxy Authentication Required</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p20492948163754"><a name="p20492948163754"></a><a name="p20492948163754"></a>You must use the proxy server for authentication so that the request can be processed.</p>
    </td>
    </tr>
    <tr id="row28680770163738"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p41441040163738"><a name="p41441040163738"></a><a name="p41441040163738"></a>408 Request Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p1281119163738"><a name="p1281119163738"></a><a name="p1281119163738"></a>The request timed out.</p>
    </td>
    </tr>
    <tr id="row65552906164354"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p8185203164354"><a name="p8185203164354"></a><a name="p8185203164354"></a>409 Conflict</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p59021712164354"><a name="p59021712164354"></a><a name="p59021712164354"></a>The request could not be processed due to a conflict.</p>
    </td>
    </tr>
    <tr id="row19714506"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p53371190"><a name="p53371190"></a><a name="p53371190"></a>500 Internal Server Error</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p28099101"><a name="p28099101"></a><a name="p28099101"></a>Failed to complete the request because of an internal service error.</p>
    </td>
    </tr>
    <tr id="row32688750164938"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p30543097164938"><a name="p30543097164938"></a><a name="p30543097164938"></a>501 Not Implemented</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p58071768164938"><a name="p58071768164938"></a><a name="p58071768164938"></a>Failed to complete the request because the server does not support the requested function.</p>
    </td>
    </tr>
    <tr id="row11809518164943"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p17046908164943"><a name="p17046908164943"></a><a name="p17046908164943"></a>502 Bad Gateway</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p38622347164943"><a name="p38622347164943"></a><a name="p38622347164943"></a>Failed to complete the request because the request is invalid.</p>
    </td>
    </tr>
    <tr id="row38399341164956"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p23338889164956"><a name="p23338889164956"></a><a name="p23338889164956"></a>503 Service Unavailable</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p11401882164956"><a name="p11401882164956"></a><a name="p11401882164956"></a>Failed to complete the request because the service is unavailable.</p>
    </td>
    </tr>
    <tr id="row51565323"><td class="cellrowborder" valign="top" width="43.419999999999995%" headers="mcps1.1.3.1.1 "><p id="p16041657"><a name="p16041657"></a><a name="p16041657"></a>504 Gateway Timeout</p>
    </td>
    <td class="cellrowborder" valign="top" width="56.58%" headers="mcps1.1.3.1.2 "><p id="p24305815"><a name="p24305815"></a><a name="p24305815"></a>A gateway timeout error occurred.</p>
    </td>
    </tr>
    </tbody>
    </table>


## Error Code<a name="section1362310255432"></a>

For details, see  [Error Codes](error-codes.md).

