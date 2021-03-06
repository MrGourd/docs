# Modifying an Agency<a name="en-us_topic_0079467623"></a>

## Function Description<a name="s6430ed804a884cada7d14960ca63f76a"></a>

This interface is used to modify agency information, including the  **trust\_domain\_id**,  **description**, and  **trust\_domain\_name**  parameters.

## URI<a name="s8cbca8f54c8d43bb9e28199dd9ad2a81"></a>

-   URI format

    PUT /v3.0/OS-AGENCY/agencies/\{agency\_id\}


-   URI parameter description

    <a name="t0cf6a030292e4bce80d74ffa2d1284a1"></a>
    <table><thead align="left"><tr id="r9fc11702a5c4477ca5e07717c151fcdd"><th class="cellrowborder" valign="top" width="19.63196319631963%" id="mcps1.1.5.1.1"><p id="a21b8e6a3cca44a5ab05b51fb7c304198"><a name="a21b8e6a3cca44a5ab05b51fb7c304198"></a><a name="a21b8e6a3cca44a5ab05b51fb7c304198"></a><strong id="en-us_topic_0026586105_b842352706143612"><a name="en-us_topic_0026586105_b842352706143612"></a><a name="en-us_topic_0026586105_b842352706143612"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="16.321632163216325%" id="mcps1.1.5.1.2"><p id="a85cfc25ffe3047bb9a203550fdac0e54"><a name="a85cfc25ffe3047bb9a203550fdac0e54"></a><a name="a85cfc25ffe3047bb9a203550fdac0e54"></a><strong id="b84235270616358_1"><a name="b84235270616358_1"></a><a name="b84235270616358_1"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="17.491749174917494%" id="mcps1.1.5.1.3"><p id="a929d26d055ce4750952eb49f41011ee4"><a name="a929d26d055ce4750952eb49f41011ee4"></a><a name="a929d26d055ce4750952eb49f41011ee4"></a><strong id="b842352706143526_1"><a name="b842352706143526_1"></a><a name="b842352706143526_1"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="46.55465546554656%" id="mcps1.1.5.1.4"><p id="a93ec0b3283ef46a19362493b7bc82d60"><a name="a93ec0b3283ef46a19362493b7bc82d60"></a><a name="a93ec0b3283ef46a19362493b7bc82d60"></a><strong id="b20601766145329_1"><a name="b20601766145329_1"></a><a name="b20601766145329_1"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r155ce3880571452bae31d4df0a643766"><td class="cellrowborder" valign="top" width="19.63196319631963%" headers="mcps1.1.5.1.1 "><p id="a5af0aceba0684973b54d926a4ccf907d"><a name="a5af0aceba0684973b54d926a4ccf907d"></a><a name="a5af0aceba0684973b54d926a4ccf907d"></a>agency_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.321632163216325%" headers="mcps1.1.5.1.2 "><p id="a5cdedfd5c9ca4ee6b67bfc49ce9fb5fe"><a name="a5cdedfd5c9ca4ee6b67bfc49ce9fb5fe"></a><a name="a5cdedfd5c9ca4ee6b67bfc49ce9fb5fe"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.491749174917494%" headers="mcps1.1.5.1.3 "><p id="a9eca7bdf93534abb92aa10ab8bc42479"><a name="a9eca7bdf93534abb92aa10ab8bc42479"></a><a name="a9eca7bdf93534abb92aa10ab8bc42479"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.55465546554656%" headers="mcps1.1.5.1.4 "><p id="a28fbce48e6aa4101b4499a282f475111"><a name="a28fbce48e6aa4101b4499a282f475111"></a><a name="a28fbce48e6aa4101b4499a282f475111"></a>ID of an agency.</p>
    </td>
    </tr>
    </tbody>
    </table>


## Request<a name="s390e257157f448b0ba10e7ca7a3cb112"></a>

-   Request header parameter description

    <a name="t541ccbfd08404d22a468e5702b497a61"></a>
    <table><thead align="left"><tr id="rfce82552c3c7432e968fd7096d56a9c2"><th class="cellrowborder" valign="top" width="19.918008199180083%" id="mcps1.1.5.1.1"><p id="a203a84a206044c7b9533bd0c7fc45a1b"><a name="a203a84a206044c7b9533bd0c7fc45a1b"></a><a name="a203a84a206044c7b9533bd0c7fc45a1b"></a><strong id="b896201652"><a name="b896201652"></a><a name="b896201652"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="16.118388161183884%" id="mcps1.1.5.1.2"><p id="a4059bc26ca7f4ecb8d4937d68ee9f47a"><a name="a4059bc26ca7f4ecb8d4937d68ee9f47a"></a><a name="a4059bc26ca7f4ecb8d4937d68ee9f47a"></a><strong id="b84235270616358_3"><a name="b84235270616358_3"></a><a name="b84235270616358_3"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="17.558244175582445%" id="mcps1.1.5.1.3"><p id="acc0a2475332b4009ad8c953fc04fbffe"><a name="acc0a2475332b4009ad8c953fc04fbffe"></a><a name="acc0a2475332b4009ad8c953fc04fbffe"></a><strong id="b842352706143526_3"><a name="b842352706143526_3"></a><a name="b842352706143526_3"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="46.405359464053596%" id="mcps1.1.5.1.4"><p id="ac5d288128c384aa49271805b68f61fc1"><a name="ac5d288128c384aa49271805b68f61fc1"></a><a name="ac5d288128c384aa49271805b68f61fc1"></a><strong id="b20601766145329_3"><a name="b20601766145329_3"></a><a name="b20601766145329_3"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r5874c77556314626aff67fb247046530"><td class="cellrowborder" valign="top" width="19.918008199180083%" headers="mcps1.1.5.1.1 "><p id="a453dda9eb4e84e7ea732bfbc54c9f4f1"><a name="a453dda9eb4e84e7ea732bfbc54c9f4f1"></a><a name="a453dda9eb4e84e7ea732bfbc54c9f4f1"></a>Content-Type</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.118388161183884%" headers="mcps1.1.5.1.2 "><p id="a02661a685b294c14a9246cc55a80e9cb"><a name="a02661a685b294c14a9246cc55a80e9cb"></a><a name="a02661a685b294c14a9246cc55a80e9cb"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.558244175582445%" headers="mcps1.1.5.1.3 "><p id="aa79d2255473641158de4ab7aa4bc55e3"><a name="aa79d2255473641158de4ab7aa4bc55e3"></a><a name="aa79d2255473641158de4ab7aa4bc55e3"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.405359464053596%" headers="mcps1.1.5.1.4 "><p id="a9966add385194e70af06e4725fecc800"><a name="a9966add385194e70af06e4725fecc800"></a><a name="a9966add385194e70af06e4725fecc800"></a>Fill <strong id="b842352706161331"><a name="b842352706161331"></a><a name="b842352706161331"></a>application/json;charset=utf8</strong> in this field.</p>
    </td>
    </tr>
    <tr id="r59de178ae38a4aa09d0be5be3a9f6725"><td class="cellrowborder" valign="top" width="19.918008199180083%" headers="mcps1.1.5.1.1 "><p id="af31b5fa207cb4d19adb7fd9003da7c4a"><a name="af31b5fa207cb4d19adb7fd9003da7c4a"></a><a name="af31b5fa207cb4d19adb7fd9003da7c4a"></a>X-Auth-Token</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.118388161183884%" headers="mcps1.1.5.1.2 "><p id="a0e5007b013ec4ecabf98c0c1aa3ddd3e"><a name="a0e5007b013ec4ecabf98c0c1aa3ddd3e"></a><a name="a0e5007b013ec4ecabf98c0c1aa3ddd3e"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.558244175582445%" headers="mcps1.1.5.1.3 "><p id="a82fd391efe4a446eaeeebef5700f86a8"><a name="a82fd391efe4a446eaeeebef5700f86a8"></a><a name="a82fd391efe4a446eaeeebef5700f86a8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.405359464053596%" headers="mcps1.1.5.1.4 "><p id="affa5c3959e014de48dac81c5be0c59ad"><a name="affa5c3959e014de48dac81c5be0c59ad"></a><a name="affa5c3959e014de48dac81c5be0c59ad"></a>Authenticated token with the <strong id="b750798910387"><a name="b750798910387"></a><a name="b750798910387"></a>Security Administrator</strong> permission.</p>
    </td>
    </tr>
    </tbody>
    </table>


-   Request body parameter description

    <a name="t6555a3e4f13a4359af5b0c60fd87ea22"></a>
    <table><thead align="left"><tr id="rc45c86da14d4406f8564d05f477cd65c"><th class="cellrowborder" valign="top" width="20.077992200779924%" id="mcps1.1.5.1.1"><p id="abaff77a5164943ca9b4bb23dcab53549"><a name="abaff77a5164943ca9b4bb23dcab53549"></a><a name="abaff77a5164943ca9b4bb23dcab53549"></a><strong id="b842352706161530"><a name="b842352706161530"></a><a name="b842352706161530"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="16.178382161783823%" id="mcps1.1.5.1.2"><p id="adf94dcaf6939468fac13e11ae027be7c"><a name="adf94dcaf6939468fac13e11ae027be7c"></a><a name="adf94dcaf6939468fac13e11ae027be7c"></a><strong id="b842352706161532"><a name="b842352706161532"></a><a name="b842352706161532"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="17.398260173982603%" id="mcps1.1.5.1.3"><p id="aece1cff828e245789017d7e9c61df39a"><a name="aece1cff828e245789017d7e9c61df39a"></a><a name="aece1cff828e245789017d7e9c61df39a"></a><strong id="b842352706143526_5"><a name="b842352706143526_5"></a><a name="b842352706143526_5"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="46.34536546345366%" id="mcps1.1.5.1.4"><p id="a7bd0ae323d0c4bf6a7938f09c3a40f1e"><a name="a7bd0ae323d0c4bf6a7938f09c3a40f1e"></a><a name="a7bd0ae323d0c4bf6a7938f09c3a40f1e"></a><strong id="b20601766145329_5"><a name="b20601766145329_5"></a><a name="b20601766145329_5"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rfafa9f4f55004ae4907c3ebea4838fcb"><td class="cellrowborder" valign="top" width="20.077992200779924%" headers="mcps1.1.5.1.1 "><p id="a14c7e4c42d804f1fbd24dccb8267f7ce"><a name="a14c7e4c42d804f1fbd24dccb8267f7ce"></a><a name="a14c7e4c42d804f1fbd24dccb8267f7ce"></a>trust_domain_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.178382161783823%" headers="mcps1.1.5.1.2 "><p id="a83ab2053f431431f8d08bc977dc6ea25"><a name="a83ab2053f431431f8d08bc977dc6ea25"></a><a name="a83ab2053f431431f8d08bc977dc6ea25"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.398260173982603%" headers="mcps1.1.5.1.3 "><p id="a23c0b7974d344da1b45284bde49100f2"><a name="a23c0b7974d344da1b45284bde49100f2"></a><a name="a23c0b7974d344da1b45284bde49100f2"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.34536546345366%" headers="mcps1.1.5.1.4 "><p id="ab3c36df6860a47ceabcf88cb9f826166"><a name="ab3c36df6860a47ceabcf88cb9f826166"></a><a name="ab3c36df6860a47ceabcf88cb9f826166"></a>ID of the delegated domain. The delegated domain must exist.</p>
    </td>
    </tr>
    <tr id="rd3dd459128d94d1abc4ac3a60bd03606"><td class="cellrowborder" valign="top" width="20.077992200779924%" headers="mcps1.1.5.1.1 "><p id="a5d2d22181d8f44b7b8ecab1a5cb16d8c"><a name="a5d2d22181d8f44b7b8ecab1a5cb16d8c"></a><a name="a5d2d22181d8f44b7b8ecab1a5cb16d8c"></a>trust_domain_name</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.178382161783823%" headers="mcps1.1.5.1.2 "><p id="a138b356fcc8f4b98af159e580d7bb664"><a name="a138b356fcc8f4b98af159e580d7bb664"></a><a name="a138b356fcc8f4b98af159e580d7bb664"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.398260173982603%" headers="mcps1.1.5.1.3 "><p id="a925e4ff5371f4ee08abeb0eb25d57995"><a name="a925e4ff5371f4ee08abeb0eb25d57995"></a><a name="a925e4ff5371f4ee08abeb0eb25d57995"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.34536546345366%" headers="mcps1.1.5.1.4 "><p id="a0fa80c97a65e4334b0fa8ce6a6370e83"><a name="a0fa80c97a65e4334b0fa8ce6a6370e83"></a><a name="a0fa80c97a65e4334b0fa8ce6a6370e83"></a>Name of the delegated domain. The delegated domain must exist.</p>
    </td>
    </tr>
    <tr id="r0331694c73854bc88e715b555b1621a5"><td class="cellrowborder" valign="top" width="20.077992200779924%" headers="mcps1.1.5.1.1 "><p id="a2b955814c61a4c49aeff45203e25a012"><a name="a2b955814c61a4c49aeff45203e25a012"></a><a name="a2b955814c61a4c49aeff45203e25a012"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.178382161783823%" headers="mcps1.1.5.1.2 "><p id="a34c0f293c02947c39207e7c493a6fb64"><a name="a34c0f293c02947c39207e7c493a6fb64"></a><a name="a34c0f293c02947c39207e7c493a6fb64"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.398260173982603%" headers="mcps1.1.5.1.3 "><p id="en-us_topic_0059029101_p733742414394"><a name="en-us_topic_0059029101_p733742414394"></a><a name="en-us_topic_0059029101_p733742414394"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.34536546345366%" headers="mcps1.1.5.1.4 "><p id="a9fada333a5b3467daff7cccc3eb34937"><a name="a9fada333a5b3467daff7cccc3eb34937"></a><a name="a9fada333a5b3467daff7cccc3eb34937"></a>Description of an agency.</p>
    </td>
    </tr>
    </tbody>
    </table>

    >![](/images/icon-note.gif) **NOTE:**   
    >The  **trust\_domain\_id**  and  **trust\_domain\_name**  parameters in a request body must exist or not exist at the same time. If both of them exist,  **trust\_domain\_name**  prevails.  


-   Sample request

    ```
    curl -i -k -H "X-Auth-Token:$token" -H 'Content-Type:application/json;charset=utf8' -X PUT -d '{"agency" : {"trust_domain_id" : "35d7706cedbc49a18df0783d00269c20","trust_domain_name" : "exampledomain","description" : "111111"}}' https://sample.domain.com/v3.0/OS-AGENCY/agencies/2809756f748a46e2b92d58d309f67291
    ```


## Response<a name="sfaeba34495564ac2bcabb59e5cf78fdb"></a>

-   Response body parameter description

    <a name="t25fa11869fcc4bbe930214e8b3a352a8"></a>
    <table><thead align="left"><tr id="r607717c6cad24f3085d946d96e8706f6"><th class="cellrowborder" valign="top" width="20.09%" id="mcps1.1.5.1.1"><p id="a60b8a28cb4a14f4d957e11fbb5ed3491"><a name="a60b8a28cb4a14f4d957e11fbb5ed3491"></a><a name="a60b8a28cb4a14f4d957e11fbb5ed3491"></a><strong id="b116474121"><a name="b116474121"></a><a name="b116474121"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="16.14%" id="mcps1.1.5.1.2"><p id="a18979c4eb8f144c889953807a71fe2c0"><a name="a18979c4eb8f144c889953807a71fe2c0"></a><a name="a18979c4eb8f144c889953807a71fe2c0"></a><strong id="b842352706161749_1"><a name="b842352706161749_1"></a><a name="b842352706161749_1"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="17.599999999999998%" id="mcps1.1.5.1.3"><p id="aac65acd7fc7b4c96933b30be7d73b987"><a name="aac65acd7fc7b4c96933b30be7d73b987"></a><a name="aac65acd7fc7b4c96933b30be7d73b987"></a><strong id="b842352706143526_7"><a name="b842352706143526_7"></a><a name="b842352706143526_7"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="46.17%" id="mcps1.1.5.1.4"><p id="ae0490d31122747f29843f4295fab3147"><a name="ae0490d31122747f29843f4295fab3147"></a><a name="ae0490d31122747f29843f4295fab3147"></a><strong id="b6981351183141_1"><a name="b6981351183141_1"></a><a name="b6981351183141_1"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rae278792d71a4337b1b3ebb9d3cee2d8"><td class="cellrowborder" valign="top" width="20.09%" headers="mcps1.1.5.1.1 "><p id="ac8b2e0e1384f4dfc8cdea40e1b2992d5"><a name="ac8b2e0e1384f4dfc8cdea40e1b2992d5"></a><a name="ac8b2e0e1384f4dfc8cdea40e1b2992d5"></a>agency</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.14%" headers="mcps1.1.5.1.2 "><p id="a3f02f98df8b4493c810f2017e8d18dd0"><a name="a3f02f98df8b4493c810f2017e8d18dd0"></a><a name="a3f02f98df8b4493c810f2017e8d18dd0"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.599999999999998%" headers="mcps1.1.5.1.3 "><p id="p5305126112619"><a name="p5305126112619"></a><a name="p5305126112619"></a>JSON object</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.17%" headers="mcps1.1.5.1.4 "><p id="p16307202622611"><a name="p16307202622611"></a><a name="p16307202622611"></a>Delegated object.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Description for the agency format

    <a name="t637ac6a0d4e945948bcb62510ba9981d"></a>
    <table><thead align="left"><tr id="red91f16bc86b42bf89be2fffd15fa889"><th class="cellrowborder" valign="top" width="20.349999999999998%" id="mcps1.1.5.1.1"><p id="a62d02d14db074ff9aed29c9a94274e1a"><a name="a62d02d14db074ff9aed29c9a94274e1a"></a><a name="a62d02d14db074ff9aed29c9a94274e1a"></a><strong id="b383334426"><a name="b383334426"></a><a name="b383334426"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="16.009999999999998%" id="mcps1.1.5.1.2"><p id="a12cc7493817349e19be4593190c9f2bd"><a name="a12cc7493817349e19be4593190c9f2bd"></a><a name="a12cc7493817349e19be4593190c9f2bd"></a><strong id="b842352706161749_3"><a name="b842352706161749_3"></a><a name="b842352706161749_3"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="17.34%" id="mcps1.1.5.1.3"><p id="a453b597a9b0a44aabffc0313debe65d0"><a name="a453b597a9b0a44aabffc0313debe65d0"></a><a name="a453b597a9b0a44aabffc0313debe65d0"></a><strong id="b842352706143526_9"><a name="b842352706143526_9"></a><a name="b842352706143526_9"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="46.300000000000004%" id="mcps1.1.5.1.4"><p id="a7a5157959ddb46a8a1c01e6cb9050aa5"><a name="a7a5157959ddb46a8a1c01e6cb9050aa5"></a><a name="a7a5157959ddb46a8a1c01e6cb9050aa5"></a><strong id="b6981351183141_3"><a name="b6981351183141_3"></a><a name="b6981351183141_3"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rfcf6c5fc35cd4850bbfe80a60139f612"><td class="cellrowborder" valign="top" width="20.349999999999998%" headers="mcps1.1.5.1.1 "><p id="a8cda852004144002a83899d4843b5bcf"><a name="a8cda852004144002a83899d4843b5bcf"></a><a name="a8cda852004144002a83899d4843b5bcf"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.2 "><p id="a8db92448d0484d269d3152dc68f2cbfb"><a name="a8db92448d0484d269d3152dc68f2cbfb"></a><a name="a8db92448d0484d269d3152dc68f2cbfb"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.34%" headers="mcps1.1.5.1.3 "><p id="a96d359bc3d664a2586371bdea61ba257"><a name="a96d359bc3d664a2586371bdea61ba257"></a><a name="a96d359bc3d664a2586371bdea61ba257"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.300000000000004%" headers="mcps1.1.5.1.4 "><p id="a7ce5115870534e1897f345bafe1d2262"><a name="a7ce5115870534e1897f345bafe1d2262"></a><a name="a7ce5115870534e1897f345bafe1d2262"></a>ID of an agency.</p>
    </td>
    </tr>
    <tr id="r15fe3d2283de41c282bc95c370547911"><td class="cellrowborder" valign="top" width="20.349999999999998%" headers="mcps1.1.5.1.1 "><p id="ac794f1663dbf4ad488f1c944a8080b98"><a name="ac794f1663dbf4ad488f1c944a8080b98"></a><a name="ac794f1663dbf4ad488f1c944a8080b98"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.2 "><p id="a45b9b9c053fa4cf7aad9ed651a19194a"><a name="a45b9b9c053fa4cf7aad9ed651a19194a"></a><a name="a45b9b9c053fa4cf7aad9ed651a19194a"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.34%" headers="mcps1.1.5.1.3 "><p id="a685ae4ba908843df99094e9ba02c73a4"><a name="a685ae4ba908843df99094e9ba02c73a4"></a><a name="a685ae4ba908843df99094e9ba02c73a4"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.300000000000004%" headers="mcps1.1.5.1.4 "><p id="a41afa278213d45009932e570b4260e2f"><a name="a41afa278213d45009932e570b4260e2f"></a><a name="a41afa278213d45009932e570b4260e2f"></a>Name of an agency.</p>
    </td>
    </tr>
    <tr id="r398c1054004a49f1a95a2f045ac90922"><td class="cellrowborder" valign="top" width="20.349999999999998%" headers="mcps1.1.5.1.1 "><p id="en-us_topic_0059029101_p27845782253"><a name="en-us_topic_0059029101_p27845782253"></a><a name="en-us_topic_0059029101_p27845782253"></a>domain_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.2 "><p id="ac4a2f900a21f4fa5a392bb31b483c61b"><a name="ac4a2f900a21f4fa5a392bb31b483c61b"></a><a name="ac4a2f900a21f4fa5a392bb31b483c61b"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.34%" headers="mcps1.1.5.1.3 "><p id="aaf88305e8cbe4ffb8d9807392ebbd331"><a name="aaf88305e8cbe4ffb8d9807392ebbd331"></a><a name="aaf88305e8cbe4ffb8d9807392ebbd331"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.300000000000004%" headers="mcps1.1.5.1.4 "><p id="a9fd0479ee3e34e53bd18e8d50a87417e"><a name="a9fd0479ee3e34e53bd18e8d50a87417e"></a><a name="a9fd0479ee3e34e53bd18e8d50a87417e"></a>ID of the current domain.</p>
    </td>
    </tr>
    <tr id="rbbd580e590c9453c89d8b75ffae226e3"><td class="cellrowborder" valign="top" width="20.349999999999998%" headers="mcps1.1.5.1.1 "><p id="ac552a537c74b43cdb5c23191b01a9866"><a name="ac552a537c74b43cdb5c23191b01a9866"></a><a name="ac552a537c74b43cdb5c23191b01a9866"></a>trust_domain_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.2 "><p id="afe8c9c1ec11d45c3a30a5e4def896fe4"><a name="afe8c9c1ec11d45c3a30a5e4def896fe4"></a><a name="afe8c9c1ec11d45c3a30a5e4def896fe4"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.34%" headers="mcps1.1.5.1.3 "><p id="ab72c799e86504b08bfab42a357d9f7b8"><a name="ab72c799e86504b08bfab42a357d9f7b8"></a><a name="ab72c799e86504b08bfab42a357d9f7b8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.300000000000004%" headers="mcps1.1.5.1.4 "><p id="a4dbd0d5deb4a414e9a23d4eda42e880a"><a name="a4dbd0d5deb4a414e9a23d4eda42e880a"></a><a name="a4dbd0d5deb4a414e9a23d4eda42e880a"></a>ID of the delegated domain.</p>
    </td>
    </tr>
    <tr id="r482f76c89cf74c8087cb46a6e56d10eb"><td class="cellrowborder" valign="top" width="20.349999999999998%" headers="mcps1.1.5.1.1 "><p id="af73b53db849d4998b890aa50a8061207"><a name="af73b53db849d4998b890aa50a8061207"></a><a name="af73b53db849d4998b890aa50a8061207"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.2 "><p id="ae7a920b0de30459bb3cd3da0cf7fd4c0"><a name="ae7a920b0de30459bb3cd3da0cf7fd4c0"></a><a name="ae7a920b0de30459bb3cd3da0cf7fd4c0"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.34%" headers="mcps1.1.5.1.3 "><p id="aa15377f5583241e6bc2df37932293f0c"><a name="aa15377f5583241e6bc2df37932293f0c"></a><a name="aa15377f5583241e6bc2df37932293f0c"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.300000000000004%" headers="mcps1.1.5.1.4 "><p id="a9cb17a7f470d4401ac242874ca368e37"><a name="a9cb17a7f470d4401ac242874ca368e37"></a><a name="a9cb17a7f470d4401ac242874ca368e37"></a>Description of an agency.</p>
    </td>
    </tr>
    <tr id="rd1bbec7a41cd4495880eebe713bd3b75"><td class="cellrowborder" valign="top" width="20.349999999999998%" headers="mcps1.1.5.1.1 "><p id="a0136c2e9eb504433ab68acb2c2d5c61b"><a name="a0136c2e9eb504433ab68acb2c2d5c61b"></a><a name="a0136c2e9eb504433ab68acb2c2d5c61b"></a>duration</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.2 "><p id="a65706c51e620413cbb29f87177165f7c"><a name="a65706c51e620413cbb29f87177165f7c"></a><a name="a65706c51e620413cbb29f87177165f7c"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.34%" headers="mcps1.1.5.1.3 "><p id="a07c033a05e244888aa5fc9a18ff1ccc8"><a name="a07c033a05e244888aa5fc9a18ff1ccc8"></a><a name="a07c033a05e244888aa5fc9a18ff1ccc8"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.300000000000004%" headers="mcps1.1.5.1.4 "><p id="p7874142115314"><a name="p7874142115314"></a><a name="p7874142115314"></a>Validity period of an agency. The default value is <strong id="b84235270615357"><a name="b84235270615357"></a><a name="b84235270615357"></a>null</strong>, indicating that the agency is permanently valid.</p>
    </td>
    </tr>
    <tr id="r41752feeccc3400286ef748488051a3a"><td class="cellrowborder" valign="top" width="20.349999999999998%" headers="mcps1.1.5.1.1 "><p id="aeafe1316400c47ac978148a484b92235"><a name="aeafe1316400c47ac978148a484b92235"></a><a name="aeafe1316400c47ac978148a484b92235"></a>expire_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.2 "><p id="a3e891583a43740e78abb0d6d55950a2b"><a name="a3e891583a43740e78abb0d6d55950a2b"></a><a name="a3e891583a43740e78abb0d6d55950a2b"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.34%" headers="mcps1.1.5.1.3 "><p id="a7b1f52ac4ecf446d824beb27b49f3496"><a name="a7b1f52ac4ecf446d824beb27b49f3496"></a><a name="a7b1f52ac4ecf446d824beb27b49f3496"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.300000000000004%" headers="mcps1.1.5.1.4 "><p id="a063b48a49a6b4c2ea7745d7111c295da"><a name="a063b48a49a6b4c2ea7745d7111c295da"></a><a name="a063b48a49a6b4c2ea7745d7111c295da"></a>Expiration time of an agency.</p>
    </td>
    </tr>
    <tr id="r29e77f7d2d4144dfbe9295612f31d5a6"><td class="cellrowborder" valign="top" width="20.349999999999998%" headers="mcps1.1.5.1.1 "><p id="a722d4fb76b4b481c88bdaf03105b150c"><a name="a722d4fb76b4b481c88bdaf03105b150c"></a><a name="a722d4fb76b4b481c88bdaf03105b150c"></a>create_time</p>
    </td>
    <td class="cellrowborder" valign="top" width="16.009999999999998%" headers="mcps1.1.5.1.2 "><p id="a9930c3c95228444797396edfd5088d43"><a name="a9930c3c95228444797396edfd5088d43"></a><a name="a9930c3c95228444797396edfd5088d43"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.34%" headers="mcps1.1.5.1.3 "><p id="a0eb080b0a1754fd293a909e7d919cbe7"><a name="a0eb080b0a1754fd293a909e7d919cbe7"></a><a name="a0eb080b0a1754fd293a909e7d919cbe7"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="46.300000000000004%" headers="mcps1.1.5.1.4 "><p id="a96a5ed6cba534a4d81e4012556b29584"><a name="a96a5ed6cba534a4d81e4012556b29584"></a><a name="a96a5ed6cba534a4d81e4012556b29584"></a>Time when an agency is created.</p>
    </td>
    </tr>
    </tbody>
    </table>


-   Sample response \(request successful\)

    ```
    {
      "agency" : {
         "description" : " testsfdas ",
         "trust_domain_id" : "3ebe1024db46485cb02ef08d3c348477",
         "id" : "c1a06ec7387f430c8122d6f336c66dcf",
         "duration" : null,
         "create_time" : "2017-01-06T05:56:09.738212",
         "expire_time" : null,
         "domain_id" : "0ae9c6993a2e47bb8c4c7a9bb8278d61",
         "name" : "exampleagency"
        }
    }
    ```


-   Sample response \(request failed\)

    ```
    {
      "error": {
        "message": "TrustDomainNotFound",
        "code": 404,
        "title": "Not Found"
      }
    }
    ```


## **Status Codes**<a name="sdfb5790305824c7f97b16547716792f2"></a>

<a name="t63bb29a8c441438e932276ef96407839"></a>
<table><thead align="left"><tr id="r6f4108d5c9ab4e2997febf132cb5e490"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="ae886f9e8fd8749059eab56cfeb402b0c"><a name="ae886f9e8fd8749059eab56cfeb402b0c"></a><a name="ae886f9e8fd8749059eab56cfeb402b0c"></a><strong id="b842352706183230_3"><a name="b842352706183230_3"></a><a name="b842352706183230_3"></a>Status Code</strong></p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="a5f5f42dcf6bf4293a55391c41db48bc4"><a name="a5f5f42dcf6bf4293a55391c41db48bc4"></a><a name="a5f5f42dcf6bf4293a55391c41db48bc4"></a><strong id="b20601766145329_7"><a name="b20601766145329_7"></a><a name="b20601766145329_7"></a>Description</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="raaded7ba0f464640a5cd98664103955a"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a893b4e2465b34681a5b446db1451412b"><a name="a893b4e2465b34681a5b446db1451412b"></a><a name="a893b4e2465b34681a5b446db1451412b"></a>200</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a28a6dd89bc5d42a880dd3ee9a2a7724d"><a name="a28a6dd89bc5d42a880dd3ee9a2a7724d"></a><a name="a28a6dd89bc5d42a880dd3ee9a2a7724d"></a>The request is successful.</p>
</td>
</tr>
<tr id="r97eb9d3bf958496fb9683db86d125989"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="ab11f8a3fcc8e4360b868e4ded87e1197"><a name="ab11f8a3fcc8e4360b868e4ded87e1197"></a><a name="ab11f8a3fcc8e4360b868e4ded87e1197"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="aeca2f2fa5a3c4457b8fb664a6d07645e"><a name="aeca2f2fa5a3c4457b8fb664a6d07645e"></a><a name="aeca2f2fa5a3c4457b8fb664a6d07645e"></a>The server failed to process the request.</p>
</td>
</tr>
<tr id="rb44296ef293d4f2abc2ad98494e19946"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="ab33518f3e43d457a985561c8fda2a2d9"><a name="ab33518f3e43d457a985561c8fda2a2d9"></a><a name="ab33518f3e43d457a985561c8fda2a2d9"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a650c2715e2224a44aa71f95f52f3bfb9"><a name="a650c2715e2224a44aa71f95f52f3bfb9"></a><a name="a650c2715e2224a44aa71f95f52f3bfb9"></a>You must enter a username and password to access the requested page.</p>
</td>
</tr>
<tr id="r9d87d9b77bdc422ca9a4bc96a14f5fec"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a22c622574b4b47f79cdeeb4ff0c4bc3a"><a name="a22c622574b4b47f79cdeeb4ff0c4bc3a"></a><a name="a22c622574b4b47f79cdeeb4ff0c4bc3a"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a529fa0478da9452db7fb4401749f1580"><a name="a529fa0478da9452db7fb4401749f1580"></a><a name="a529fa0478da9452db7fb4401749f1580"></a>You are forbidden to access the requested page.</p>
</td>
</tr>
<tr id="row1248231194611"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p1648193117462"><a name="p1648193117462"></a><a name="p1648193117462"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p1748113194616"><a name="p1748113194616"></a><a name="p1748113194616"></a>The server could not find the requested page.</p>
</td>
</tr>
<tr id="r54d808c8ee8a48bd921c839b88d5c28b"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="aa858e87d17bf4ef3b95698ba4b57e7c5"><a name="aa858e87d17bf4ef3b95698ba4b57e7c5"></a><a name="aa858e87d17bf4ef3b95698ba4b57e7c5"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a1ddbe1581e9d4e8e9e7d3539a32ac5d5"><a name="a1ddbe1581e9d4e8e9e7d3539a32ac5d5"></a><a name="a1ddbe1581e9d4e8e9e7d3539a32ac5d5"></a>Failed to complete the request because of an internal service error.</p>
</td>
</tr>
</tbody>
</table>

