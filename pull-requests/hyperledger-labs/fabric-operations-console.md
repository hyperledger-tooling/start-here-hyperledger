---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    add prefix to random ids and log it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                don't merge yet - saving code for next week

Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

- Improvement - will log that we created a random deployer component id.


#### Description
this helps us debug where the id came from.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 17:52:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    add mustgather strings to localization file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 17:43:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    add skip param to restore api + rebuild white list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This adds a skip doc query parameter to the restore api. This will allow use of the restore api w/o having to modify the backup object in order to NOT restore certain documents.

This PR also rebuilds the component whitelist once a restore is complete.  This should allow the console to operate with the components found in its db.

query params:
```js
skip_system="['00_settings_athena']"	// [optional] docs that match these ids will not be restored to the system db
skip_component="['abcd']"	// [optional] docs that match these ids will not be restored to the components db
```
Signed-off-by: David Huffman <dshuffma@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 20:39:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/98" class=".btn">#98</a>
            </td>
            <td>
                <b>
                    issues template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 18:43:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/97" class=".btn">#97</a>
            </td>
            <td>
                <b>
                    updated release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 15:44:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    add a read-only-mode server setting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                read only mode will allow users to view/monitor components/ledger, but they will be unable to create new or edit existing components.

Signed-off-by: David Huffman <dshuffma@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 21:42:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Fix auto fabric upgrade parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The auto fabric upgrade logic was not parsing the get-available-fabric-versions api response correctly, causes the upgrade api to fail.

This PR also now ignores the db setting `DISABLE_AUTO_FAB_UP` when calling the fabric upgrade manually. meaning the setting `DISABLE_AUTO_FAB_UP` only applies to the automatic fabric upgrade logic.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 20:53:36 +0000 UTC
    </div>
</div>

