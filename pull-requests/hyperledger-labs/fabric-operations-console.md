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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/241" class=".btn">#241</a>
            </td>
            <td>
                <b>
                    remove the identity drop down in the join flow
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

- chooses the correct identity for the join osn flow, uses the same logic as the get-config-block code
- removes the drop down to select an identity for the join osn flow


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-02 01:43:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    Fix orderer node join to channel
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
- Fixes the join orderer to a channel panel when the orderer does not have a system channel.
- Removed the join orderer to a channel code from the create wizard. the join-osn modal is now used instead.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-01 19:43:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/238" class=".btn">#238</a>
            </td>
            <td>
                <b>
                    fix msp import if there are no intermediate_certs
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
Fixes an error when importing a MSP json file with no `intermediate_certs` field. This field can be blank or missing and the import should still succeed.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 18:17:59 +0000 UTC
    </div>
</div>

