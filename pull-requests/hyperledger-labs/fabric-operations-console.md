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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    add orderer org signature step on channel edit
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
Adds the orderer org signature setep (when its needed) during the channel update wizard.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 21:12:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    parse config block Endpoints -> addressess safely
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
Handle empty or undefined values for  `Endpoints.value.addresses` in a config block. This fixes an error when joining a peer to a channel that has an orderer org with zero orderers.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 18:12:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    remove restart on admin cert change
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
Removes unnecessary component restart on an admin cert change.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 17:44:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    send restart for each comp that has a new tls cert
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
Fixes issue where orderers & peers are not restarting after clicking `Update associated nodes` after a TLS cert was updated on a CA.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 17:41:40 +0000 UTC
    </div>
</div>

