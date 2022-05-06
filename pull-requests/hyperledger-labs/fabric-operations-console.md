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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Updated tag to software-login for Login feature file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ketul Shah <shah.ketul@ibm.com>

#### Type of change
- Test update

#### Description
Updated tag @saas for Login feature file

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 05:35:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    remove the confusing part of the error message
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
Remove the part of the error message that only applies if you were using the APIs.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 18:52:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    restyle audit button so its not invisible
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
The audit notification button was styled in a way that made it invisible.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 17:58:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    do not run k8s sync w/cached deployer data
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
The cached deployer data cannot be used to synchronize the state of the component. It should be skipped, unless the real (up-to-date) data was obtained.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-03 19:25:57 +0000 UTC
    </div>
</div>

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

