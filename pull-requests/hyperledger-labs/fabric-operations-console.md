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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/113" class=".btn">#113</a>
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
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 17:49:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    log if the deployer id came from the api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement 


#### Description
adds log message that the deployer id came from the api request.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 17:46:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    allow associating identities from intermediate ca
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
This pr allows identities from an intermediate CA to be available in the associate drop down.
https://github.com/hyperledger-labs/fabric-operations-console/issues/109


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 19:41:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    fix refresh cert button, only show for deploy node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

- Bug fix

#### Description
The "refresh cert" button should show up for deployed nodes and not show for imported nodes. This was not working as intended for orderering nodes. If the first orderer in an OS (when sorted by name alphabetically) was a deployed node, the console would show the button on all ordering nodes in that OS.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-15 19:34:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    lint code
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

- Improvement 

#### Description
- linted code based on es lint rules

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 20:34:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    use the same major and minor versions for upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

- use the same major and minor versions for upgrade

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 20:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    add react route for exporting identities via link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

- New feature

#### Description
adds a route to download the identities. visiting `/export-identities` will immediately prompt for a local download of your wallet.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 21:38:32 +0000 UTC
    </div>
</div>

