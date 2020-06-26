# Querying the Service Catalog<a name="iam_02_0004"></a>

## Function Description<a name="s81394c6441e2433aa089b83d9ae901bb"></a>

This interface is used to query the service catalog corresponding to  **X-Auth-Token**  contained in the request.

## URI<a name="s7f773a8bf34349f5bf81d0c7af9a440d"></a>

URI format

GET /v3/auth/catalog

## **Request**<a name="sf86f3f4f84a8493e84f564c16c53eaf3"></a>

-   Request header parameter description

    <a name="tab13448d4b644cd482b72e023e311a4c"></a>
    <table><thead align="left"><tr id="r9cc8c45e565f499a85068ccf812c4906"><th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.1"><p id="en-us_topic_0031136110_p289771511147"><a name="en-us_topic_0031136110_p289771511147"></a><a name="en-us_topic_0031136110_p289771511147"></a><strong id="b37426530113629"><a name="b37426530113629"></a><a name="b37426530113629"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.2"><p id="aa8a52be628254fb799e7d667253339cf"><a name="aa8a52be628254fb799e7d667253339cf"></a><a name="aa8a52be628254fb799e7d667253339cf"></a><strong id="ac429376f11ae472b87ff4be326afb9d8"><a name="ac429376f11ae472b87ff4be326afb9d8"></a><a name="ac429376f11ae472b87ff4be326afb9d8"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.3"><p id="a8de3dfc3143a4304a1273fade5a53dae"><a name="a8de3dfc3143a4304a1273fade5a53dae"></a><a name="a8de3dfc3143a4304a1273fade5a53dae"></a><strong id="b842352706143526_3"><a name="b842352706143526_3"></a><a name="b842352706143526_3"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="25%" id="mcps1.1.5.1.4"><p id="a51fedaacfb0744a39c0e39893bf93f94"><a name="a51fedaacfb0744a39c0e39893bf93f94"></a><a name="a51fedaacfb0744a39c0e39893bf93f94"></a><strong id="b14438018113629"><a name="b14438018113629"></a><a name="b14438018113629"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r80e6b051a95142239d52ef85b3b9e59c"><td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.1 "><p id="a88f9db0a7b6c4b4690378ccf5a787f60"><a name="a88f9db0a7b6c4b4690378ccf5a787f60"></a><a name="a88f9db0a7b6c4b4690378ccf5a787f60"></a>X-Auth-Token</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.2 "><p id="ad6cfd0f57eb643a0afb40a639b4a8515"><a name="ad6cfd0f57eb643a0afb40a639b4a8515"></a><a name="ad6cfd0f57eb643a0afb40a639b4a8515"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.3 "><p id="ac4cc17eda4bf4dd4aa34a5449be8f04e"><a name="ac4cc17eda4bf4dd4aa34a5449be8f04e"></a><a name="ac4cc17eda4bf4dd4aa34a5449be8f04e"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="25%" headers="mcps1.1.5.1.4 "><p id="a259cd575002145db850a7dcaf1cbe007"><a name="a259cd575002145db850a7dcaf1cbe007"></a><a name="a259cd575002145db850a7dcaf1cbe007"></a>Authenticated scoped token of a project.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Sample request

    ```
    curl -i -k -H 'Accept:application/json' -H 'X-Auth-Token:$token' -H 'Content-Type:application/json;charset=utf8' -X GET https://iam.example.com/v3/auth/catalog
    ```


## **Response**<a name="s6e8a35fa777c4de29b376bef459aba1d"></a>

Sample response \(successful request\)

```
{
  "catalog": [
    {
      "endpoints": [
        {
          "region_id": null,
          "url": "https://172.30.49.68:7443/v2/c972a59e958e407e89b0c6d8e522df3b",
          "region": null,
          "interface": "public",
          "id": "04f0ee42038447f0a9c7b407028fd7b9"
        }
      ],
      "type": "compute",
      "id": "eb884e9f64b44dd0ac73cdc55d817286",
      "name": "nova"
    }
  ],
  "links": {
    "self": "https://iam.example.com/v3/auth/catalog"
  }
}
```

## **Status Codes**<a name="s161ee4f22c7a4e5f928bf049a4425742"></a>

<a name="en-us_topic_0031136110_table25927028"></a>
<table><thead align="left"><tr id="en-us_topic_0031136110_row10578662"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="en-us_topic_0031136110_p51565323"><a name="en-us_topic_0031136110_p51565323"></a><a name="en-us_topic_0031136110_p51565323"></a><strong id="b37151362163018"><a name="b37151362163018"></a><a name="b37151362163018"></a>Status Code</strong></p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="en-us_topic_0031136110_p16041657"><a name="en-us_topic_0031136110_p16041657"></a><a name="en-us_topic_0031136110_p16041657"></a><strong id="b38470707163018"><a name="b38470707163018"></a><a name="b38470707163018"></a>Description</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="en-us_topic_0031136110_row24305815"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0031136110_p22613965"><a name="en-us_topic_0031136110_p22613965"></a><a name="en-us_topic_0031136110_p22613965"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="en-us_topic_0031136110_p19791876"><a name="en-us_topic_0031136110_p19791876"></a><a name="en-us_topic_0031136110_p19791876"></a>The request is successful.</p>
</td>
</tr>
<tr id="en-us_topic_0031136110_row43909159"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0031136110_p66980994"><a name="en-us_topic_0031136110_p66980994"></a><a name="en-us_topic_0031136110_p66980994"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="en-us_topic_0031136110_p56751409"><a name="en-us_topic_0031136110_p56751409"></a><a name="en-us_topic_0031136110_p56751409"></a>The server failed to process the request.</p>
</td>
</tr>
<tr id="re5868592b58a49148d1e374ab0ee4186"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a67da088f332e48ca9c70f3ba30897dde"><a name="a67da088f332e48ca9c70f3ba30897dde"></a><a name="a67da088f332e48ca9c70f3ba30897dde"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a0525ff08629b4648808d6e876aaf9c5f"><a name="a0525ff08629b4648808d6e876aaf9c5f"></a><a name="a0525ff08629b4648808d6e876aaf9c5f"></a>You must enter a username and password to access the requested page.</p>
</td>
</tr>
<tr id="en-us_topic_0031136110_row41000636"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0031136110_p32717189"><a name="en-us_topic_0031136110_p32717189"></a><a name="en-us_topic_0031136110_p32717189"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a98f74bf5eda646c6a5973dfa742126c4"><a name="a98f74bf5eda646c6a5973dfa742126c4"></a><a name="a98f74bf5eda646c6a5973dfa742126c4"></a>You are forbidden to access the requested page.</p>
</td>
</tr>
<tr id="r40e82c2469d34bf089fe9bfb0fa81526"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a8be4e075b25144a38cbe0ff05c2b2f15"><a name="a8be4e075b25144a38cbe0ff05c2b2f15"></a><a name="a8be4e075b25144a38cbe0ff05c2b2f15"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a5147e7c96ca94cb882828f2c4a33c1dc"><a name="a5147e7c96ca94cb882828f2c4a33c1dc"></a><a name="a5147e7c96ca94cb882828f2c4a33c1dc"></a>The server could not find the requested page.</p>
</td>
</tr>
<tr id="r6ae77ec5e12645e0a53aa0f3be73d1a9"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a61cb90ae8ac1482f83a82028556bbee5"><a name="a61cb90ae8ac1482f83a82028556bbee5"></a><a name="a61cb90ae8ac1482f83a82028556bbee5"></a>405</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a41bd1c94c1ba4153b7346917bc58b6b3"><a name="a41bd1c94c1ba4153b7346917bc58b6b3"></a><a name="a41bd1c94c1ba4153b7346917bc58b6b3"></a>You are not allowed to use the method specified in the request.</p>
</td>
</tr>
<tr id="rbea4e490c384410e8d1210ca41179e16"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a9eaf1c04680e4901822818bfe53ee0fc"><a name="a9eaf1c04680e4901822818bfe53ee0fc"></a><a name="a9eaf1c04680e4901822818bfe53ee0fc"></a>413</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a5e2acac6d93f406caa8cb7f89f4b0e4d"><a name="a5e2acac6d93f406caa8cb7f89f4b0e4d"></a><a name="a5e2acac6d93f406caa8cb7f89f4b0e4d"></a>The request entity is too large.</p>
</td>
</tr>
<tr id="r3b34616283144b19899b01b4552b799c"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a898bb41bdd874b25b452c9fd609e5bc0"><a name="a898bb41bdd874b25b452c9fd609e5bc0"></a><a name="a898bb41bdd874b25b452c9fd609e5bc0"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="ad43eae2906e84b6fb48fb6c11746dfab"><a name="ad43eae2906e84b6fb48fb6c11746dfab"></a><a name="ad43eae2906e84b6fb48fb6c11746dfab"></a>Failed to complete the request because of an internal service error.</p>
</td>
</tr>
<tr id="r73ae10963ce24ea09cafcfec5f21c2ab"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a3f2f513363a24dcb87462518dff622e7"><a name="a3f2f513363a24dcb87462518dff622e7"></a><a name="a3f2f513363a24dcb87462518dff622e7"></a>503</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a642a35bd05f24df68588a7f13c7cb3b7"><a name="a642a35bd05f24df68588a7f13c7cb3b7"></a><a name="a642a35bd05f24df68588a7f13c7cb3b7"></a>Failed to complete the request because the service is unavailable.</p>
</td>
</tr>
</tbody>
</table>

