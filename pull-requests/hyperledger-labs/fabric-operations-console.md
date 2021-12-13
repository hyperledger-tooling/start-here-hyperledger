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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    update release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                updating release notes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 19:07:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    fix version compare logic with double digit str
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description
The version comparison logic did not work correctly when comparing 1 double digit version to a single digit version.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 18:56:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    1208-releasenotes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- release notes

#### Description
- updated release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 21:55:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/102" class=".btn">#102</a>
            </td>
            <td>
                <b>
                    Auto upgrade version fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Bug fix

#### Description
- the auto upgrade fabric logic was upgrading from versions that were okay. it was upgrading all orderers to the highest available major fabric version, unless they were already at the highest level (within the same major version).


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 18:59:15 +0000 UTC
    </div>
</div>

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

