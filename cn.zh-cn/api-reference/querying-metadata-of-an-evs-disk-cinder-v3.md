# Querying Metadata of an EVS Disk<a name="evs_04_3039"></a>

## Function<a name="section19390540"></a>

This API is used to query the metadata of an EVS disk.

## URI<a name="section40297137"></a>

-   URI format

    GET /v3/\{project\_id\}/volumes/\{volume\_id\}/metadata

-   Parameter description

    <a name="table8745607"></a>
    <table><thead align="left"><tr id="row15985080"><th class="cellrowborder" valign="top" width="31.069999999999997%" id="mcps1.1.4.1.1"><p id="p19723089"><a name="p19723089"></a><a name="p19723089"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="17.919999999999998%" id="mcps1.1.4.1.2"><p id="p54066375"><a name="p54066375"></a><a name="p54066375"></a>Mandatory</p>
    </th>
    <th class="cellrowborder" valign="top" width="51.01%" id="mcps1.1.4.1.3"><p id="p17300225"><a name="p17300225"></a><a name="p17300225"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row59140967"><td class="cellrowborder" valign="top" width="31.069999999999997%" headers="mcps1.1.4.1.1 "><p id="p25689059"><a name="p25689059"></a><a name="p25689059"></a>project_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.919999999999998%" headers="mcps1.1.4.1.2 "><p id="p439002"><a name="p439002"></a><a name="p439002"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p35559222"><a name="p35559222"></a><a name="p35559222"></a>Specifies the project ID.</p>
    </td>
    </tr>
    <tr id="row51597550"><td class="cellrowborder" valign="top" width="31.069999999999997%" headers="mcps1.1.4.1.1 "><p id="p18651996"><a name="p18651996"></a><a name="p18651996"></a>volume_id</p>
    </td>
    <td class="cellrowborder" valign="top" width="17.919999999999998%" headers="mcps1.1.4.1.2 "><p id="p34416674"><a name="p34416674"></a><a name="p34416674"></a>Yes</p>
    </td>
    <td class="cellrowborder" valign="top" width="51.01%" headers="mcps1.1.4.1.3 "><p id="p36287209"><a name="p36287209"></a><a name="p36287209"></a>Specifies the disk ID.</p>
    </td>
    </tr>
    </tbody>
    </table>


## Request<a name="section27129916"></a>

-   Example request

    ```
    GET https://{endpoint}/v3/{project_id}/volumes/{volume_id}/metadata
    ```


## Response<a name="section42842654"></a>

-   Parameter description

    <a name="evs_04_2075_table11977025201856"></a>
    <table><thead align="left"><tr id="evs_04_2075_row8102228201856"><th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.1"><p id="evs_04_2075_p52300707201856"><a name="evs_04_2075_p52300707201856"></a><a name="evs_04_2075_p52300707201856"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.43%" id="mcps1.1.4.1.2"><p id="evs_04_2075_p3642697315541"><a name="evs_04_2075_p3642697315541"></a><a name="evs_04_2075_p3642697315541"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.14%" id="mcps1.1.4.1.3"><p id="evs_04_2075_p17319263201856"><a name="evs_04_2075_p17319263201856"></a><a name="evs_04_2075_p17319263201856"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2075_row60683035201856"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2075_p16378828201856"><a name="evs_04_2075_p16378828201856"></a><a name="evs_04_2075_p16378828201856"></a>metadata</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2075_p6490369115541"><a name="evs_04_2075_p6490369115541"></a><a name="evs_04_2075_p6490369115541"></a>Object</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2075_p20205612201856"><a name="evs_04_2075_p20205612201856"></a><a name="evs_04_2075_p20205612201856"></a>Specifies the disk metadata, which is made up of key-value pairs.</p>
    </td>
    </tr>
    <tr id="evs_04_2075_row108939111229"><td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.1 "><p id="evs_04_2075_p129522216412"><a name="evs_04_2075_p129522216412"></a><a name="evs_04_2075_p129522216412"></a>error</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.43%" headers="mcps1.1.4.1.2 "><p id="evs_04_2075_p1595262111415"><a name="evs_04_2075_p1595262111415"></a><a name="evs_04_2075_p1595262111415"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.14%" headers="mcps1.1.4.1.3 "><p id="evs_04_2075_p109527215417"><a name="evs_04_2075_p109527215417"></a><a name="evs_04_2075_p109527215417"></a>Specifies the error message returned when an error occurs. For details, see <a href="#evs_04_2075_li0419202382514">Parameters in the error field</a>.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   <a name="evs_04_2075_li0419202382514"></a>Parameters in the  **error**  field

    <a name="evs_04_2075_evs_04_2013_table15441099103019"></a>
    <table><thead align="left"><tr id="evs_04_2075_evs_04_2013_row54094047103019"><th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.1"><p id="evs_04_2075_evs_04_2013_p19541716103019"><a name="evs_04_2075_evs_04_2013_p19541716103019"></a><a name="evs_04_2075_evs_04_2013_p19541716103019"></a>Parameter</p>
    </th>
    <th class="cellrowborder" valign="top" width="21.17788221177882%" id="mcps1.1.4.1.2"><p id="evs_04_2075_evs_04_2013_p39375186103019"><a name="evs_04_2075_evs_04_2013_p39375186103019"></a><a name="evs_04_2075_evs_04_2013_p39375186103019"></a>Type</p>
    </th>
    <th class="cellrowborder" valign="top" width="57.64423557644236%" id="mcps1.1.4.1.3"><p id="evs_04_2075_evs_04_2013_p38578950103019"><a name="evs_04_2075_evs_04_2013_p38578950103019"></a><a name="evs_04_2075_evs_04_2013_p38578950103019"></a>Description</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="evs_04_2075_evs_04_2013_row59401790103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2075_evs_04_2013_p46815658103019"><a name="evs_04_2075_evs_04_2013_p46815658103019"></a><a name="evs_04_2075_evs_04_2013_p46815658103019"></a>message</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2075_evs_04_2013_p33971979103019"><a name="evs_04_2075_evs_04_2013_p33971979103019"></a><a name="evs_04_2075_evs_04_2013_p33971979103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2075_evs_04_2013_p21623243103019"><a name="evs_04_2075_evs_04_2013_p21623243103019"></a><a name="evs_04_2075_evs_04_2013_p21623243103019"></a>Specifies the error message returned when an error occurs.</p>
    </td>
    </tr>
    <tr id="evs_04_2075_evs_04_2013_row60391466103019"><td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.1 "><p id="evs_04_2075_evs_04_2013_p59870541103019"><a name="evs_04_2075_evs_04_2013_p59870541103019"></a><a name="evs_04_2075_evs_04_2013_p59870541103019"></a>code</p>
    </td>
    <td class="cellrowborder" valign="top" width="21.17788221177882%" headers="mcps1.1.4.1.2 "><p id="evs_04_2075_evs_04_2013_p17675690103019"><a name="evs_04_2075_evs_04_2013_p17675690103019"></a><a name="evs_04_2075_evs_04_2013_p17675690103019"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="57.64423557644236%" headers="mcps1.1.4.1.3 "><p id="evs_04_2075_evs_04_2013_p6087468103019"><a name="evs_04_2075_evs_04_2013_p6087468103019"></a><a name="evs_04_2075_evs_04_2013_p6087468103019"></a>Specifies the error code returned when an error occurs.</p>
    <p id="evs_04_2075_evs_04_2013_p54787218103019"><a name="evs_04_2075_evs_04_2013_p54787218103019"></a><a name="evs_04_2075_evs_04_2013_p54787218103019"></a>For details about the error code, see <a href="error-codes.md">Error Codes</a>.</p>
    </td>
    </tr>
    </tbody>
    </table>

-   Example response

    ```
    {
        "metadata": {
            "key1": "value1", 
            "key2": "value2"
        }
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

    In the preceding example,  **error**  indicates a general error, for example,  **badrequest**  or  **itemNotFound**. An example is provided as follows:

    ```
    {
        "badrequest": {
            "message": "XXXX", 
            "code": "XXX"
        }
    }
    ```


## Status Codes<a name="section50039568"></a>

-   Normal

    200


## Error Codes<a name="section431317151242"></a>

For details, see  [Error Codes](error-codes.md).

