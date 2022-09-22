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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/307" class=".btn">#307</a>
            </td>
            <td>
                <b>
                    add npm flag to fix build with react deps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The command `npm ci` is failing under apollo, due to conflicting react dependency versions. this fixes the error by ignoring it.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-19 19:06:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/306" class=".btn">#306</a>
            </td>
            <td>
                <b>
                    add migration apis for status and db migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
This is part of a wider unreleased feature to migrate console from one console to another. These apis are complete, but are not usable until the migration component is done.

- added api to get  overall migration status
- added api to migrate databases to new console


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 18:57:40 +0000 UTC
    </div>
</div>

