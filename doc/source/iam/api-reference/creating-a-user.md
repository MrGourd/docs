# Creating a User<a name="en-us_topic_0057845637"></a>

## Function Description<a name="s5888597838b0425a92e3419fb766c7f5"></a>

This interface is used to create a user under a domain.

## URI<a name="s46d3616bd4c54e55ba97a528518a5890"></a>

URI format

POST /v3/users

## Request<a name="se7fe5cac0d544e119c49322cc1707eb6"></a>

-   Request header parameter description

    <a name="t68c7bd10e66a4380a1e6cdc78ca95669"></a>
    <table><thead align="left"><tr id="r584496594a404ce18918a40e6e57c2ec"><th class="cellrowborder" valign="top" width="21.95%" id="mcps1.1.5.1.1"><p id="ac3a989cc5d3a405889eabb47dee84b04"><a name="ac3a989cc5d3a405889eabb47dee84b04"></a><a name="ac3a989cc5d3a405889eabb47dee84b04"></a><strong id="a6f95694edbbb43d8a152536754b86c82_1"><a name="a6f95694edbbb43d8a152536754b86c82_1"></a><a name="a6f95694edbbb43d8a152536754b86c82_1"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="20.75%" id="mcps1.1.5.1.2"><p id="a69a20ac00b86496aa8418517c542b0da"><a name="a69a20ac00b86496aa8418517c542b0da"></a><a name="a69a20ac00b86496aa8418517c542b0da"></a><strong id="a105e6ed8c3de4c5a9dde97ae5a71071e_1"><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_1"></a><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_1"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="20.169999999999998%" id="mcps1.1.5.1.3"><p id="a92c23d4441054df0972e025aeb3a8d7f"><a name="a92c23d4441054df0972e025aeb3a8d7f"></a><a name="a92c23d4441054df0972e025aeb3a8d7f"></a><strong id="a703d34a49a2f4162bc1a1a439f655f95_1"><a name="a703d34a49a2f4162bc1a1a439f655f95_1"></a><a name="a703d34a49a2f4162bc1a1a439f655f95_1"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="37.13%" id="mcps1.1.5.1.4"><p id="abe6882c44cf4402d8ed7706b9278f33b"><a name="abe6882c44cf4402d8ed7706b9278f33b"></a><a name="abe6882c44cf4402d8ed7706b9278f33b"></a><strong id="b842352706114032_1"><a name="b842352706114032_1"></a><a name="b842352706114032_1"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="r5d63069d6a8a426e8b25b94d1b4d302a"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="ad4fb6253385c46ab8720a0e13f573694"><a name="ad4fb6253385c46ab8720a0e13f573694"></a><a name="ad4fb6253385c46ab8720a0e13f573694"></a>Content-Type</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.1.5.1.2 "><p id="a6b33800bcb2a446695b1d33a2d751554"><a name="a6b33800bcb2a446695b1d33a2d751554"></a><a name="a6b33800bcb2a446695b1d33a2d751554"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.169999999999998%" headers="mcps1.1.5.1.3 "><p id="ab34a5e95b76b4b79a72da0734025f211"><a name="ab34a5e95b76b4b79a72da0734025f211"></a><a name="ab34a5e95b76b4b79a72da0734025f211"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.13%" headers="mcps1.1.5.1.4 "><p id="a716277ae541d4553bb10490f9c02593d"><a name="a716277ae541d4553bb10490f9c02593d"></a><a name="a716277ae541d4553bb10490f9c02593d"></a>Fill <strong id="b842352706161331"><a name="b842352706161331"></a><a name="b842352706161331"></a>application/json;charset=utf8</strong> in this field.</p>
    </td>
    </tr>
    <tr id="row29501427115257"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="p6637478211538"><a name="p6637478211538"></a><a name="p6637478211538"></a>X-Auth-Token</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.75%" headers="mcps1.1.5.1.2 "><p id="p764826811538"><a name="p764826811538"></a><a name="p764826811538"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.169999999999998%" headers="mcps1.1.5.1.3 "><p id="p1553001111538"><a name="p1553001111538"></a><a name="p1553001111538"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.13%" headers="mcps1.1.5.1.4 "><p id="p53757920173238"><a name="p53757920173238"></a><a name="p53757920173238"></a>Authenticated token with the <strong id="b750798910387"><a name="b750798910387"></a><a name="b750798910387"></a>Security Administrator</strong> permission.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Request body parameter description

    <a name="en-us_topic_0026585112_table59995477"></a>
    <table><thead align="left"><tr id="en-us_topic_0026585112_row14620943"><th class="cellrowborder" valign="top" width="22.13%" id="mcps1.1.5.1.1"><p id="en-us_topic_0026585112_p43445707"><a name="en-us_topic_0026585112_p43445707"></a><a name="en-us_topic_0026585112_p43445707"></a><strong id="b57378080173054"><a name="b57378080173054"></a><a name="b57378080173054"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="20.71%" id="mcps1.1.5.1.2"><p id="en-us_topic_0026585112_p29441404"><a name="en-us_topic_0026585112_p29441404"></a><a name="en-us_topic_0026585112_p29441404"></a><strong id="a105e6ed8c3de4c5a9dde97ae5a71071e_3"><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_3"></a><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_3"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="19.78%" id="mcps1.1.5.1.3"><p id="en-us_topic_0026585112_p35943562"><a name="en-us_topic_0026585112_p35943562"></a><a name="en-us_topic_0026585112_p35943562"></a><strong id="a703d34a49a2f4162bc1a1a439f655f95_3"><a name="a703d34a49a2f4162bc1a1a439f655f95_3"></a><a name="a703d34a49a2f4162bc1a1a439f655f95_3"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="37.38%" id="mcps1.1.5.1.4"><p id="en-us_topic_0026585112_p25747420"><a name="en-us_topic_0026585112_p25747420"></a><a name="en-us_topic_0026585112_p25747420"></a><strong id="b111517773914474"><a name="b111517773914474"></a><a name="b111517773914474"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row42114291102223"><td class="cellrowborder" valign="top" width="22.13%" headers="mcps1.1.5.1.1 "><p id="p53974141102228"><a name="p53974141102228"></a><a name="p53974141102228"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.71%" headers="mcps1.1.5.1.2 "><p id="p57978071102228"><a name="p57978071102228"></a><a name="p57978071102228"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.3 "><p id="p21086678102228"><a name="p21086678102228"></a><a name="p21086678102228"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.38%" headers="mcps1.1.5.1.4 "><p id="p63231356193217"><a name="p63231356193217"></a><a name="p63231356193217"></a>A username with 5 to 32 characters. The username can contain special characters, but only hyphens (-), underscores (_), and periods (.) are allowed. It cannot start with a digit.</p>
    </td>
    </tr>
    <tr id="row37810320102744"><td class="cellrowborder" valign="top" width="22.13%" headers="mcps1.1.5.1.1 "><p id="p42737049102744"><a name="p42737049102744"></a><a name="p42737049102744"></a>domain_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.71%" headers="mcps1.1.5.1.2 "><p id="p39148906102744"><a name="p39148906102744"></a><a name="p39148906102744"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.3 "><p id="p16944812102744"><a name="p16944812102744"></a><a name="p16944812102744"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.38%" headers="mcps1.1.5.1.4 "><p id="p30352518102744"><a name="p30352518102744"></a><a name="p30352518102744"></a>ID of the domain where a user is located.</p>
    </td>
    </tr>
    <tr id="row15919216102748"><td class="cellrowborder" valign="top" width="22.13%" headers="mcps1.1.5.1.1 "><p id="p14388120102748"><a name="p14388120102748"></a><a name="p14388120102748"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.71%" headers="mcps1.1.5.1.2 "><p id="p24587085102748"><a name="p24587085102748"></a><a name="p24587085102748"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.3 "><p id="p45396854102748"><a name="p45396854102748"></a><a name="p45396854102748"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.38%" headers="mcps1.1.5.1.4 "><p id="p107415910126"><a name="p107415910126"></a><a name="p107415910126"></a>Whether a user is enabled.</p>
    <p id="p53266556102748"><a name="p53266556102748"></a><a name="p53266556102748"></a>The value can be <strong id="b18570608618403"><a name="b18570608618403"></a><a name="b18570608618403"></a>true</strong> or <strong id="b65172625518403"><a name="b65172625518403"></a><a name="b65172625518403"></a>false</strong>. <strong id="b127154530118403"><a name="b127154530118403"></a><a name="b127154530118403"></a>true</strong> indicates the user is enabled and <strong id="b173784535818403"><a name="b173784535818403"></a><a name="b173784535818403"></a>false</strong> indicates the user is not enabled. The default value is <strong id="b842352706184016"><a name="b842352706184016"></a><a name="b842352706184016"></a>true</strong>.</p>
    </td>
    </tr>
    <tr id="row12436720103234"><td class="cellrowborder" valign="top" width="22.13%" headers="mcps1.1.5.1.1 "><p id="p741379103234"><a name="p741379103234"></a><a name="p741379103234"></a>password</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.71%" headers="mcps1.1.5.1.2 "><p id="p60051710103234"><a name="p60051710103234"></a><a name="p60051710103234"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.3 "><p id="p32350346103234"><a name="p32350346103234"></a><a name="p32350346103234"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.38%" headers="mcps1.1.5.1.4 "><div class="p" id="p35681422175348"><a name="p35681422175348"></a><a name="p35681422175348"></a>Password of the user. The password must meet the following requirements:<a name="ul62058101036"></a><a name="ul62058101036"></a><ul id="ul62058101036"><li>Can contain 6 to 32 characters. The system default minimum password length is 6 characters, and you can change the minimum password length.</li><li>Must contain at least two of the following character types: uppercase letters, lowercase letters, digits, and special characters.</li><li>Cannot be the username or the username spelled backwards.</li><li>Cannot contain the user's mobile phone number or email address.</li><li>Must comply with the password policies under <strong id="b842352706162030"><a name="b842352706162030"></a><a name="b842352706162030"></a>Account Settings</strong>.</li></ul>
    </div>
    </td>
    </tr>
    <tr id="row32792190161256"><td class="cellrowborder" valign="top" width="22.13%" headers="mcps1.1.5.1.1 "><p id="p38921737161256"><a name="p38921737161256"></a><a name="p38921737161256"></a>default_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.71%" headers="mcps1.1.5.1.2 "><p id="p65652968161256"><a name="p65652968161256"></a><a name="p65652968161256"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.3 "><p id="p16290180161256"><a name="p16290180161256"></a><a name="p16290180161256"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.38%" headers="mcps1.1.5.1.4 "><p id="p44436164161256"><a name="p44436164161256"></a><a name="p44436164161256"></a>Default project ID of a user.</p>
    </td>
    </tr>
    <tr id="row37051718182711"><td class="cellrowborder" valign="top" width="22.13%" headers="mcps1.1.5.1.1 "><p id="p3493194592314"><a name="p3493194592314"></a><a name="p3493194592314"></a>description</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.71%" headers="mcps1.1.5.1.2 "><p id="p1649374552312"><a name="p1649374552312"></a><a name="p1649374552312"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.78%" headers="mcps1.1.5.1.3 "><p id="p1049316456234"><a name="p1049316456234"></a><a name="p1049316456234"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.38%" headers="mcps1.1.5.1.4 "><p id="p134931945102313"><a name="p134931945102313"></a><a name="p134931945102313"></a>Description of the user.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Sample request

    ```
    1. Create the temporary file ${filename}.json based on the following template. ${filename} indicates the temporary file name, which is user-defined.
    {
        "user": {
            "default_project_id": "acf2ffabba974fae8f30378ffde2cfa6",
            "domain_id": "88b16b6440684467b8825d7d96e154d8",
            "enabled": true,
            "name": "jamesdoe",
            "password": "********"
        }
    }
    2. Run the following command under the directory of the ${filename}.json file.
    curl -i -k -H 'Accept:application/json' -H 'Content-Type:application/json;charset=utf8' -H "X-Auth-Token:$token" -X POST -d @${filename}.json https://172.30.48.86:31943/v3/users
    3. Run the following command under the directory of the ${filename}.json file to delete the ${filename}.json file.
    rm ${filename}.json
    ```


## Response<a name="s3a08e13bb5b34dc2ba4dcd84a0d51cf5"></a>

-   Response body parameter description

    <a name="t1266dd240c3649048c9f42af34a0686b"></a>
    <table><thead align="left"><tr id="rd8ac2cd80e4b47d684b61df4f3c570cf"><th class="cellrowborder" valign="top" width="22.08%" id="mcps1.1.5.1.1"><p id="ad167d1bf89ca443eac693ea562da12a3"><a name="ad167d1bf89ca443eac693ea562da12a3"></a><a name="ad167d1bf89ca443eac693ea562da12a3"></a><strong id="a6f95694edbbb43d8a152536754b86c82_3"><a name="a6f95694edbbb43d8a152536754b86c82_3"></a><a name="a6f95694edbbb43d8a152536754b86c82_3"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="20.77%" id="mcps1.1.5.1.2"><p id="aad08ea1f8c8e4a42a1a81112a74cb237"><a name="aad08ea1f8c8e4a42a1a81112a74cb237"></a><a name="aad08ea1f8c8e4a42a1a81112a74cb237"></a><strong id="a105e6ed8c3de4c5a9dde97ae5a71071e_5"><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_5"></a><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_5"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="20.01%" id="mcps1.1.5.1.3"><p id="a9b5fafff0348408893dcc06fbe0b1186"><a name="a9b5fafff0348408893dcc06fbe0b1186"></a><a name="a9b5fafff0348408893dcc06fbe0b1186"></a><strong id="a703d34a49a2f4162bc1a1a439f655f95_5"><a name="a703d34a49a2f4162bc1a1a439f655f95_5"></a><a name="a703d34a49a2f4162bc1a1a439f655f95_5"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="37.14%" id="mcps1.1.5.1.4"><p id="ad002a0bf107a468884a5777e55f837f6"><a name="ad002a0bf107a468884a5777e55f837f6"></a><a name="ad002a0bf107a468884a5777e55f837f6"></a><strong id="b842352706114032_3"><a name="b842352706114032_3"></a><a name="b842352706114032_3"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="ref3b81e8e64e418c961ca1bce6f25280"><td class="cellrowborder" valign="top" width="22.08%" headers="mcps1.1.5.1.1 "><p id="abb2b4d81b907497da50ad4f12760f7dc"><a name="abb2b4d81b907497da50ad4f12760f7dc"></a><a name="abb2b4d81b907497da50ad4f12760f7dc"></a>user</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.77%" headers="mcps1.1.5.1.2 "><p id="a7e49a4eaca054e36ba774b0cdc492081"><a name="a7e49a4eaca054e36ba774b0cdc492081"></a><a name="a7e49a4eaca054e36ba774b0cdc492081"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="20.01%" headers="mcps1.1.5.1.3 "><p id="p1527211816218"><a name="p1527211816218"></a><a name="p1527211816218"></a>JSON object</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.14%" headers="mcps1.1.5.1.4 "><p id="a8ded0409c6d948dc82f7f779a4cfa5b8"><a name="a8ded0409c6d948dc82f7f779a4cfa5b8"></a><a name="a8ded0409c6d948dc82f7f779a4cfa5b8"></a>User object.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Description for the user format

    <a name="t3ef10d134105438f922a72ac36adbe13"></a>
    <table><thead align="left"><tr id="ra836795da3204436ad115c6d63f33cb3"><th class="cellrowborder" valign="top" width="21.95%" id="mcps1.1.5.1.1"><p id="a915f4fa2492a4fa3b5fc5b52cb975ed3"><a name="a915f4fa2492a4fa3b5fc5b52cb975ed3"></a><a name="a915f4fa2492a4fa3b5fc5b52cb975ed3"></a><strong id="a6f95694edbbb43d8a152536754b86c82_5"><a name="a6f95694edbbb43d8a152536754b86c82_5"></a><a name="a6f95694edbbb43d8a152536754b86c82_5"></a>Parameter</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="21.15%" id="mcps1.1.5.1.2"><p id="aeb29128c8bc6489593aaf12297635c52"><a name="aeb29128c8bc6489593aaf12297635c52"></a><a name="aeb29128c8bc6489593aaf12297635c52"></a><strong id="a105e6ed8c3de4c5a9dde97ae5a71071e_7"><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_7"></a><a name="a105e6ed8c3de4c5a9dde97ae5a71071e_7"></a>Mandatory</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="19.63%" id="mcps1.1.5.1.3"><p id="a367df15999ce47aa8fa2550bb2d3df9a"><a name="a367df15999ce47aa8fa2550bb2d3df9a"></a><a name="a367df15999ce47aa8fa2550bb2d3df9a"></a><strong id="a703d34a49a2f4162bc1a1a439f655f95_7"><a name="a703d34a49a2f4162bc1a1a439f655f95_7"></a><a name="a703d34a49a2f4162bc1a1a439f655f95_7"></a>Type</strong></p>
    </th>
    <th class="cellrowborder" valign="top" width="37.269999999999996%" id="mcps1.1.5.1.4"><p id="a16a6b7e4145e4fbabf25e75163ec3f95"><a name="a16a6b7e4145e4fbabf25e75163ec3f95"></a><a name="a16a6b7e4145e4fbabf25e75163ec3f95"></a><strong id="b842352706114032_5"><a name="b842352706114032_5"></a><a name="b842352706114032_5"></a>Description</strong></p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="rb2ba995189ec478eb5d1181d3bb7be1c"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="aa1005da54f2c4746ae99676d14ab012d"><a name="aa1005da54f2c4746ae99676d14ab012d"></a><a name="aa1005da54f2c4746ae99676d14ab012d"></a>enabled</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.5.1.2 "><p id="a6d0540b177e34775b18c670cf5cd46bc"><a name="a6d0540b177e34775b18c670cf5cd46bc"></a><a name="a6d0540b177e34775b18c670cf5cd46bc"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.63%" headers="mcps1.1.5.1.3 "><p id="a65f6a6fc5a364d868072c58eeab90325"><a name="a65f6a6fc5a364d868072c58eeab90325"></a><a name="a65f6a6fc5a364d868072c58eeab90325"></a>Boolean</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.269999999999996%" headers="mcps1.1.5.1.4 "><p id="p1544652451214"><a name="p1544652451214"></a><a name="p1544652451214"></a>Whether a user is enabled.</p>
    <p id="ababe5d21d4764e209d225a4cea9b9fa2"><a name="ababe5d21d4764e209d225a4cea9b9fa2"></a><a name="ababe5d21d4764e209d225a4cea9b9fa2"></a>The value can be <strong id="b1249664277"><a name="b1249664277"></a><a name="b1249664277"></a>true</strong> or <strong id="b2065514822"><a name="b2065514822"></a><a name="b2065514822"></a>false</strong>. <strong id="b1440197199"><a name="b1440197199"></a><a name="b1440197199"></a>true</strong> indicates the user is enabled and <strong id="b683968503"><a name="b683968503"></a><a name="b683968503"></a>false</strong> indicates the user is not enabled. The default value is <strong id="b819911535"><a name="b819911535"></a><a name="b819911535"></a>true</strong>.</p>
    </td>
    </tr>
    <tr id="r41522dc2bd8d475b8d2a16af17d5213b"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="a2501c5b12ff94e338c0930e6c321af90"><a name="a2501c5b12ff94e338c0930e6c321af90"></a><a name="a2501c5b12ff94e338c0930e6c321af90"></a>id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.5.1.2 "><p id="af10224f581d946cb91a49683adf34271"><a name="af10224f581d946cb91a49683adf34271"></a><a name="af10224f581d946cb91a49683adf34271"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.63%" headers="mcps1.1.5.1.3 "><p id="a0316e95fb756489a82f70ae562c523b4"><a name="a0316e95fb756489a82f70ae562c523b4"></a><a name="a0316e95fb756489a82f70ae562c523b4"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.269999999999996%" headers="mcps1.1.5.1.4 "><p id="af5ce8c5c520f468895f28d74f6eb4540"><a name="af5ce8c5c520f468895f28d74f6eb4540"></a><a name="af5ce8c5c520f468895f28d74f6eb4540"></a>User ID.</p>
    </td>
    </tr>
    <tr id="r1208cbb1496440d89eb758b2cd80d578"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="a4504807eb899465fb0ce3ac82d7013dc"><a name="a4504807eb899465fb0ce3ac82d7013dc"></a><a name="a4504807eb899465fb0ce3ac82d7013dc"></a>domain_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.5.1.2 "><p id="en-us_topic_0026585113_p386591205643"><a name="en-us_topic_0026585113_p386591205643"></a><a name="en-us_topic_0026585113_p386591205643"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.63%" headers="mcps1.1.5.1.3 "><p id="a293aacc9b5354786a8b30a063a186b02"><a name="a293aacc9b5354786a8b30a063a186b02"></a><a name="a293aacc9b5354786a8b30a063a186b02"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.269999999999996%" headers="mcps1.1.5.1.4 "><p id="aa1138dcdd40340039e621e7abf0332e1"><a name="aa1138dcdd40340039e621e7abf0332e1"></a><a name="aa1138dcdd40340039e621e7abf0332e1"></a>ID of the domain where a user is located.</p>
    </td>
    </tr>
    <tr id="rbe8775b4e77a4b08be093de05e7bcbf3"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="acc4c499e1b2f4bdd98e5c7acd4e8861b"><a name="acc4c499e1b2f4bdd98e5c7acd4e8861b"></a><a name="acc4c499e1b2f4bdd98e5c7acd4e8861b"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.5.1.2 "><p id="a4bf5dfe715d342e0a883343cbcf8181a"><a name="a4bf5dfe715d342e0a883343cbcf8181a"></a><a name="a4bf5dfe715d342e0a883343cbcf8181a"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.63%" headers="mcps1.1.5.1.3 "><p id="a8c424bac7d93444dbc647a1d5c5c21e4"><a name="a8c424bac7d93444dbc647a1d5c5c21e4"></a><a name="a8c424bac7d93444dbc647a1d5c5c21e4"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.269999999999996%" headers="mcps1.1.5.1.4 "><p id="afc48731c8a2e4c66a56ac245f7a1e34e"><a name="afc48731c8a2e4c66a56ac245f7a1e34e"></a><a name="afc48731c8a2e4c66a56ac245f7a1e34e"></a>Username.</p>
    </td>
    </tr>
    <tr id="row884150412952"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="p4507320312952"><a name="p4507320312952"></a><a name="p4507320312952"></a>links</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.5.1.2 "><p id="p2705079812952"><a name="p2705079812952"></a><a name="p2705079812952"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.63%" headers="mcps1.1.5.1.3 "><p id="p192144107220"><a name="p192144107220"></a><a name="p192144107220"></a>JSON object</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.269999999999996%" headers="mcps1.1.5.1.4 "><p id="p4445286212952"><a name="p4445286212952"></a><a name="p4445286212952"></a>Resource links of a user.</p>
    </td>
    </tr>
    <tr id="row451303512957"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="p3001154112957"><a name="p3001154112957"></a><a name="p3001154112957"></a>default_project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.5.1.2 "><p id="p1501577612957"><a name="p1501577612957"></a><a name="p1501577612957"></a>No</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.63%" headers="mcps1.1.5.1.3 "><p id="p831835612957"><a name="p831835612957"></a><a name="p831835612957"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.269999999999996%" headers="mcps1.1.5.1.4 "><p id="p269819912957"><a name="p269819912957"></a><a name="p269819912957"></a>Default project ID of a user.</p>
    </td>
    </tr>
    <tr id="row62718260507"><td class="cellrowborder" valign="top" width="21.95%" headers="mcps1.1.5.1.1 "><p id="p192802695014"><a name="p192802695014"></a><a name="p192802695014"></a>password_expires_at</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.15%" headers="mcps1.1.5.1.2 "><p id="p14282026125012"><a name="p14282026125012"></a><a name="p14282026125012"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="19.63%" headers="mcps1.1.5.1.3 "><p id="p202852615016"><a name="p202852615016"></a><a name="p202852615016"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="37.269999999999996%" headers="mcps1.1.5.1.4 "><p id="p228162616501"><a name="p228162616501"></a><a name="p228162616501"></a>UTC when the password will expire. <strong id="b1483686226114627"><a name="b1483686226114627"></a><a name="b1483686226114627"></a>null</strong> indicates that the password will not expire.</p>
    </td>
    </tr>
    </tbody>
    </table>


-   Sample response

    ```
    {
        "user": {
            "name": "jamesdoe",
            "links": {
                "self": "https://sample.domain.com/v3/users/614d1d2fb86940faab8f350bf1b9dbac"
            },
            "domain_id": "88b16b6440684467b8825d7d96e154d8",
            "enabled": true,
            "id": "614d1d2fb86940faab8f350bf1b9dbac",
            "default_project_id": "acf2ffabba974fae8f30378ffde2cfa6",
            "password_expires_at": null
        }
    }
    ```


## Status Codes<a name="sbfe93ca4c2b9427dbb2218a4e72da6a8"></a>

<a name="en-us_topic_0035544336_table25927028"></a>
<table><thead align="left"><tr id="en-us_topic_0035544336_row10578662"><th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.1"><p id="en-us_topic_0035544336_p51565323"><a name="en-us_topic_0035544336_p51565323"></a><a name="en-us_topic_0035544336_p51565323"></a><strong id="b842352706104328"><a name="b842352706104328"></a><a name="b842352706104328"></a>Status Code</strong></p>
</th>
<th class="cellrowborder" valign="top" width="50%" id="mcps1.1.3.1.2"><p id="en-us_topic_0035544336_p16041657"><a name="en-us_topic_0035544336_p16041657"></a><a name="en-us_topic_0035544336_p16041657"></a><strong id="b842352706114032_7"><a name="b842352706114032_7"></a><a name="b842352706114032_7"></a>Description</strong></p>
</th>
</tr>
</thead>
<tbody><tr id="en-us_topic_0035544336_row24305815"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0035544336_p22613965"><a name="en-us_topic_0035544336_p22613965"></a><a name="en-us_topic_0035544336_p22613965"></a>201</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="en-us_topic_0035544336_p19791876"><a name="en-us_topic_0035544336_p19791876"></a><a name="en-us_topic_0035544336_p19791876"></a>The user is successfully created.</p>
</td>
</tr>
<tr id="en-us_topic_0035544336_row43909159"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0035544336_p66980994"><a name="en-us_topic_0035544336_p66980994"></a><a name="en-us_topic_0035544336_p66980994"></a>400</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="en-us_topic_0035544336_p56751409"><a name="en-us_topic_0035544336_p56751409"></a><a name="en-us_topic_0035544336_p56751409"></a>The server failed to process the request.</p>
</td>
</tr>
<tr id="rb99fbab78bc54ae4953661763b573830"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="aef55745ff0834933af36d690e2e339b8"><a name="aef55745ff0834933af36d690e2e339b8"></a><a name="aef55745ff0834933af36d690e2e339b8"></a>401</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a480215738ced4bf5a8feafa2681db93b"><a name="a480215738ced4bf5a8feafa2681db93b"></a><a name="a480215738ced4bf5a8feafa2681db93b"></a>You must enter a username and password to access the requested page.</p>
</td>
</tr>
<tr id="en-us_topic_0035544336_row41000636"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="en-us_topic_0035544336_p32717189"><a name="en-us_topic_0035544336_p32717189"></a><a name="en-us_topic_0035544336_p32717189"></a>403</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="ae678037f26d640f5a985c943e2ffb92e"><a name="ae678037f26d640f5a985c943e2ffb92e"></a><a name="ae678037f26d640f5a985c943e2ffb92e"></a>You are forbidden to access the requested page.</p>
</td>
</tr>
<tr id="r1fd5c05b7b6b4c048f3f7b9ddbc755b0"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a5d7e2305922e4f9098442a900792dae1"><a name="a5d7e2305922e4f9098442a900792dae1"></a><a name="a5d7e2305922e4f9098442a900792dae1"></a>404</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a9edf299d0513460caaac8a2a19b76e9a"><a name="a9edf299d0513460caaac8a2a19b76e9a"></a><a name="a9edf299d0513460caaac8a2a19b76e9a"></a>The server could not find the requested page.</p>
</td>
</tr>
<tr id="rbb5133f150fd42eebde8dd6e390ecbd5"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="ad1a2754016e44193a97043265cd611cf"><a name="ad1a2754016e44193a97043265cd611cf"></a><a name="ad1a2754016e44193a97043265cd611cf"></a>405</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a81837d461ef445259c5a6e9e1ce0e32a"><a name="a81837d461ef445259c5a6e9e1ce0e32a"></a><a name="a81837d461ef445259c5a6e9e1ce0e32a"></a>You are not allowed to use the method specified in the request.</p>
</td>
</tr>
<tr id="row59784631174446"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="p10716980174446"><a name="p10716980174446"></a><a name="p10716980174446"></a>409</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="p62769041174446"><a name="p62769041174446"></a><a name="p62769041174446"></a>A resource conflict occurs.</p>
</td>
</tr>
<tr id="r2cecff297b1a412f956a312d3cd7acc9"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a1f617621d1bc4a9facb1c84d1946002b"><a name="a1f617621d1bc4a9facb1c84d1946002b"></a><a name="a1f617621d1bc4a9facb1c84d1946002b"></a>413</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="ac31ead3ee2db40eea8ae45b2779a09e9"><a name="ac31ead3ee2db40eea8ae45b2779a09e9"></a><a name="ac31ead3ee2db40eea8ae45b2779a09e9"></a>The request entity is too large.</p>
</td>
</tr>
<tr id="rd71e0e00759f4179a2dccaf345ba9f2f"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a1657c5ca5ebd4a2cbacbdb35fc9b7601"><a name="a1657c5ca5ebd4a2cbacbdb35fc9b7601"></a><a name="a1657c5ca5ebd4a2cbacbdb35fc9b7601"></a>500</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a88b4b14048564e12942b8151dc791b99"><a name="a88b4b14048564e12942b8151dc791b99"></a><a name="a88b4b14048564e12942b8151dc791b99"></a>Failed to complete the request because of an internal service error.</p>
</td>
</tr>
<tr id="r5647e5fd26974514ac66cc3925f30601"><td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.1 "><p id="a16dfaa16ceac4a33a468c0ae158292fb"><a name="a16dfaa16ceac4a33a468c0ae158292fb"></a><a name="a16dfaa16ceac4a33a468c0ae158292fb"></a>503</p>
</td>
<td class="cellrowborder" valign="top" width="50%" headers="mcps1.1.3.1.2 "><p id="a5635c1924d9648a8be89b1e5dcf0a87b"><a name="a5635c1924d9648a8be89b1e5dcf0a87b"></a><a name="a5635c1924d9648a8be89b1e5dcf0a87b"></a>Failed to complete the request because the service is unavailable.</p>
</td>
</tr>
</tbody>
</table>

