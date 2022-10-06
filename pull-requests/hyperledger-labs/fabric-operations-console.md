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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/320" class=".btn">#320</a>
            </td>
            <td>
                <b>
                    Migration Completion Banner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: selvaprakash92 <selvaprakash92@gmail.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description

To Notify the completion of Migration and Further steps


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-06 11:06:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/318" class=".btn">#318</a>
            </td>
            <td>
                <b>
                    Bug fix when adding ordering nodes to channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Modem <Nikhil.Modem@ibm.com>

#### Type of change
- Bug fix

#### Description
- If an ordering cluster has nodes with the system channel, they were available to add to a channel. The entire cluster should not show up in this case.
- If an ordering cluster has nodes both with and without the system channel, all node were available to add to the channel. The cluster should show up, but only the nodes that do not have a system channel should show up in this case.
- Both of the above scenarios are dealt with by only returning nodes that do not have a system channel, regardless of the overall cluster configuration.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-05 16:47:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    change start command
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
There is some sort of permission error, trying to change the start command from `npm start` to `node server_watcher.js`.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-03 14:12:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/316" class=".btn">#316</a>
            </td>
            <td>
                <b>
                    change fabric links from 1.4 to 2.4
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

- Documentation update

#### Description
Move some Fabric documentation links to the latest release.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 19:54:52 +0000 UTC
    </div>
</div>

