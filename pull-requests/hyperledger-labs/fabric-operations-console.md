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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    npm updates for stitch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

- Dep updates

#### Description
Npm dependency updates


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 20:00:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    remove hardcoded title text, use product label str
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
- The base text for the browser tab title was hard coded. This fixes that and uses the product string.
- npm dep updates


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 19:09:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    check that admin cert is from one of the root CAs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change
- Bug fix

#### Description
If you upload an admin cert into MSP that did not come from one of the root CAs, when the cert gets uploaded to the peer, the peer will crash. Ensure that the admin certs are from one of the root (or intermediate) CAs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-06 14:07:50 +0000 UTC
    </div>
</div>

