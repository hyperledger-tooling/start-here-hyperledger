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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    fix the advanced create channel step logic
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
- fixes the step enable/disable logic in the advanced create channel wizard


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 22:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Fix signature auth - channel creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
 - Fixed an issue with a missing msp id that fails to build a proper signature authorize field. Happens during channel creation.
 - Adds some server side logs to help identify the missing msp id issue
 - Adds case sensitive flag to fabric gateway config-override validation (unrelated to channel issue)
 - Fixed issue where the application/orderer/channel capabilities were being set on a create-channel flow causing create failures.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 17:44:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    fix create channel button
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
One of the wizard changes for the new features was breaking the normal create channel button.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 13:33:13 +0000 UTC
    </div>
</div>

