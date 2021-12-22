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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/114" class=".btn">#114</a>
            </td>
            <td>
                <b>
                    fix the available fabric upgrade  w/old versions
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
This PR fixes the "fabric upgrade available" code if the component is using a short hand version field. 

Older components may have a version of `"v1.4"` instead of the major.minor.patch-prerelease format like `"1.4.5-6"`. The short hand version fields break the "upgrade available" logic (it won't prompt for a fabric upgrade).


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-20 20:19:42 +0000 UTC
    </div>
</div>

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

