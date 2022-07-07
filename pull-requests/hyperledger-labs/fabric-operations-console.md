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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    fix get-channels logic if response is empty
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

- fixes the response to get-osn-channels when there are 0 channels. makes it an empty array instead of null.
- fixes `system_channel_id` filed being set to null, should be empty string when there is no system channel


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 14:47:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    Updated test case to create orderer with system channel
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
Updated test case to create orderer with system channel
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 13:18:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/247" class=".btn">#247</a>
            </td>
            <td>
                <b>
                    add the consenters to review step of create channel wizard
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
- show the consenter node ids in the review panel of the create channel wizard.
- surface block parsing or getting errors in join osn wizard


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 21:00:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/246" class=".btn">#246</a>
            </td>
            <td>
                <b>
                    added the system channel removal doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
added the system channel removal doc


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 20:02:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/245" class=".btn">#245</a>
            </td>
            <td>
                <b>
                    Fix systemless detection
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
- Fix the with or without system channel detection in the orderer details page
- Adds orderer type to side panel in orderer details page
- Fix the loading logic in the orderer details page
- Updates the node's `systemless` field after removing system channel

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 18:49:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    fix title bar on login page
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
The browser's title bar on the login page was not always correct


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 20:51:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    only join selected orderers to channel
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
Only join the orderers that were checked to the channel


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 20:10:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    improve warning msg and fix os details tab logic
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
- Improves the "TLS identity not found" warning message on the orderer cluster details page. adds why this message is appearing and how to fix it
- Fixes logic on the orderer cluster details page showing the wrong content


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 19:59:35 +0000 UTC
    </div>
</div>

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

