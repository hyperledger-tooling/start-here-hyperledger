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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    add more upgrade warnings around fabric versions
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

- Improvement (improvement to code, performance, etc)

#### Description
- Adds an error on more *peer*  upgrade flows. 
- Adds parameter to ignore upgrade errors and force an update

Upgrades that will throw an error:

- from 1.4.x to 2.4.x 
- from 2.0.x to 2.4.x 
- from 2.1.x to 2.4.x  
- from 2.2.x to 2.4.x 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 17:14:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    prevent fabric upgrades that can break chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
Upgrading fabric from 1.4 to 2.4 is dangerous. This PR prevents it on the UI and on APIs. Also shows the warning/description.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-28 18:27:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    add a default app capability when creating channel
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
When creating a channel with default settings, a default application capability was accidentally left off.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 17:22:07 +0000 UTC
    </div>
</div>

