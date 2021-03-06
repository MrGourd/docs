# Creating a Bucket<a name="obs_03_0306"></a>

This section describes how to create a bucket on OBS Console. A bucket is a container that stores objects in OBS. Before you store data in OBS, you need to create a bucket.

>![](public_sys-resources/icon-note.gif) **NOTE:** 
>On OBS Console, an account can have 100 buckets. There is no such upper limit if you use the API or other methods to create buckets. However, these buckets also take up the bucket quota on OBS Console.

## Procedure<a name="sb79f841ab9af4b9faf6cbad1932c33b0"></a>

1.  In the upper right corner of the OBS Console homepage, click  **Create Bucket**. The  **Create Bucket**  page is displayed. For details, see  [Figure 1](#fig30207295194414).

    **Figure  1**  Creating a bucket<a name="fig30207295194414"></a>  
    ![](figures/creating-a-bucket.png "creating-a-bucket")

2.  Configure bucket parameters.

    **Table  1**  Bucket parameters

    <a name="table9210201853617"></a>
    <table><thead align="left"><tr id="row13210518113615"><th class="cellrowborder" valign="top" width="20.22%" id="mcps1.2.3.1.1"><p id="p1121013185365"><a name="p1121013185365"></a><a name="p1121013185365"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="79.78%" id="mcps1.2.3.1.2"><p id="p20210111833619"><a name="p20210111833619"></a><a name="p20210111833619"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row721018185364"><td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.3.1.1 "><p id="p12210111812361"><a name="p12210111812361"></a><a name="p12210111812361"></a>Region</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.78%" headers="mcps1.2.3.1.2 "><p id="p480613549419"><a name="p480613549419"></a><a name="p480613549419"></a>Geographic area where a bucket resides. For low network latency and quick resource access, select the nearest region. Once a bucket is created, the region cannot be changed.</p>
    </td>
    </tr>
    <tr id="row321061820361"><td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.3.1.1 "><p id="p6210181823616"><a name="p6210181823616"></a><a name="p6210181823616"></a>Bucket Name</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.78%" headers="mcps1.2.3.1.2 "><p id="p18210191820365"><a name="p18210191820365"></a><a name="p18210191820365"></a>Name of the bucket. The bucket name must be unique across all accounts and regions. Once a bucket is created, you cannot change its name.</p>
    <p id="p404056794432"><a name="p404056794432"></a><a name="p404056794432"></a>An OBS bucket must be named according to the globally applied DNS naming rules as follows:</p>
    <a name="ul5989254594432"></a><a name="ul5989254594432"></a><ul id="ul5989254594432"><li>A bucket name must be unique across all accounts and regions.</li><li>A bucket name must contain 3 to 63 characters. Only lowercase letters, digits, hyphens (-), and periods (.) are allowed.</li><li>A bucket name cannot start or end with a period (.) or hyphen (-), and cannot contain two consecutive periods (.) or contain a period (.) and a hyphen (-) adjacent to each other.</li><li>A bucket name cannot be an IP address.</li><li>If a bucket name contains any period (.), the security certificate verification may be triggered when you access the bucket or objects in the bucket.</li></ul>
    </td>
    </tr>
    <tr id="row132101185362"><td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.3.1.1 "><p id="p18210181833614"><a name="p18210181833614"></a><a name="p18210181833614"></a>Storage Class</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.78%" headers="mcps1.2.3.1.2 "><p id="p2914586010533"><a name="p2914586010533"></a><a name="p2914586010533"></a>Storage classes of a bucket. Different storage classes meet different requirements for storage performance and costs.</p>
    <a name="ul386215378248"></a><a name="ul386215378248"></a><ul id="ul386215378248"><li>The Standard storage class features low access latency and high throughput. It is therefore suitable for storing a massive number of hot files (frequently accessed every month) or small files.</li><li>The Warm storage class is ideal for storing data that is semi-frequently accessed (less than 12 times a year), with requirements for quick response.</li><li>The Archive storage class is suitable for archiving data that is rarely-accessed (averagely once a year), without requirements for quick response.</li></ul>
    <p id="p859325514419"><a name="p859325514419"></a><a name="p859325514419"></a>For details, see <a href="storage-classes-overview-(console).md">Storage Classes Overview</a>.</p>
    </td>
    </tr>
    <tr id="row162107185362"><td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.3.1.1 "><p id="p1621051833618"><a name="p1621051833618"></a><a name="p1621051833618"></a>Bucket Policy</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.78%" headers="mcps1.2.3.1.2 "><p id="p13250952104514"><a name="p13250952104514"></a><a name="p13250952104514"></a>Controls read and write permissions for buckets.</p>
    <a name="ul3921758194016"></a><a name="ul3921758194016"></a><ul id="ul3921758194016"><li><strong id="en-us_topic_0045853745_b8759625143810"><a name="en-us_topic_0045853745_b8759625143810"></a><a name="en-us_topic_0045853745_b8759625143810"></a>Private</strong>: No access beyond the bucket ACL settings is granted.</li><li><strong id="en-us_topic_0045853745_b917713334388"><a name="en-us_topic_0045853745_b917713334388"></a><a name="en-us_topic_0045853745_b917713334388"></a>Public Read</strong>: Any user can read objects in the bucket.</li><li><strong id="en-us_topic_0045853745_b624737913162154"><a name="en-us_topic_0045853745_b624737913162154"></a><a name="en-us_topic_0045853745_b624737913162154"></a>Public Read and Write</strong>: Any user can read, write, and delete objects in the bucket.</li></ul>
    </td>
    </tr>
    <tr id="row179244845019"><td class="cellrowborder" valign="top" width="20.22%" headers="mcps1.2.3.1.1 "><p id="p1934488501"><a name="p1934488501"></a><a name="p1934488501"></a>Tags (optional)</p>
    </td>
    <td class="cellrowborder" valign="top" width="79.78%" headers="mcps1.2.3.1.2 "><p id="p293184875012"><a name="p293184875012"></a><a name="p293184875012"></a>Tags are used to identify and classify buckets in OBS. Each tag is represented by a key-value pair. For more information, see <a href="tag-overview.md">Tag Overview</a>.</p>
    </td>
    </tr>
    </tbody>
    </table>

3.  Click  **Create Now**.

