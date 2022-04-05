---
layout: default
title: fabric-chaincode-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-chaincode-node
---

# fabric-chaincode-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-chaincode-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/320" class=".btn">#320</a>
            </td>
            <td>
                <b>
                    wip - protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 09:40:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/319" class=".btn">#319</a>
            </td>
            <td>
                <b>
                    Some updates to the latest tool versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 08:49:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-chaincode-node/pull/317" class=".btn">#317</a>
            </td>
            <td>
                <b>
                    Build failure - ignorable warning not ignored
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Recent builds have failed with the browserlist module reporting
(on stderr) that it was outdated. This is a dependency of nyc, code coverage.

nyc is 'resting' and not actively being maintained.

Rush version used here is not ignoring that warning, and build fails.

Can't alter the rush rebuild command to ignore warnings. It's really
just going on anything written to stderr.

So adding a redirect on the nyc command stderr-> stdout (2>&1)
Have checked that a drop in coverage does still cause a failure.

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 08:24:20 +0000 UTC
    </div>
</div>

