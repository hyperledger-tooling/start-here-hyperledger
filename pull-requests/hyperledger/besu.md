---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6226" class=".btn">#6226</a>
            </td>
            <td>
                <b>
                    Update OpenJ9 Docker image to latest version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 18:00:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6225" class=".btn">#6225</a>
            </td>
            <td>
                <b>
                    Use `From` field in a `PING` packet when creating a peer table entry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR uses the `From` field of a `PING` packet when creating a local entry in the peer table, unless the `From` field is not available in which case it reverts to the existing behaviour of using the `UDP` source address.

## Fixed Issue(s)
Fixes https://github.com/hyperledger/besu/issues/6224
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 15:07:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6222" class=".btn">#6222</a>
            </td>
            <td>
                <b>
                    [MINOR] move Pipeline stack trace to trace/debug level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                log a message only at info
log stack trace at debug/trace depending on type of exception

fixes #5533 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 03:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6221" class=".btn">#6221</a>
            </td>
            <td>
                <b>
                    [MINOR] - Add plugin version summary
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add plugin version summary
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-01 01:55:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6218" class=".btn">#6218</a>
            </td>
            <td>
                <b>
                    Allow `maxActiveConnections` for GraphQL and terminate requests based on actual connection status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

1. The option of `--graphql-http-max-active-connections` has been added to limit the numer of GraphQL requests served each time.
2. The GraphQL server has been relying on an `isAliveHandler` to terminate requests based on the timeout. However, this handler was only applied to `matchingLogs`, resulting in unterminated GraphQL executions in general even if the connection has timed out. Rather than relying on a future task, it is more appropriate to terminate requests based on the actual status of the connection. The `TimeoutHandler` should have handled the HTTP timeout while connections may also be terminated due to exceeding `maxActiveConnections`.

Docs change would be added in another PR in a later stage when code changes stabilise.

## Fixed Issue(s)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 15:40:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6215" class=".btn">#6215</a>
            </td>
            <td>
                <b>
                    Unpin ca-certificates-java version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

CI builds are currently broken because an ubuntu package update breaks with ca-certificates-java version 20190909. If we allow it to use updates to the version (such as 20190909ubuntu1.2) the build un-breaks.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 17:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6214" class=".btn">#6214</a>
            </td>
            <td>
                <b>
                    GitHub ci testing pr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                DO NOT MERGE
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 14:49:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6212" class=".btn">#6212</a>
            </td>
            <td>
                <b>
                    [#5851] Add error messages on authentication failures with username and password
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Include in body message in response 400

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5851
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 08:44:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6210" class=".btn">#6210</a>
            </td>
            <td>
                <b>
                    Don't disconnect if insufficient peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">peering</span>
            </td>
            <td>
                Don't do any outbound disconnects if EthPeers count is below maxPeers

With these changes, while below maxPeers, the only disconnects that happen with established peers are those found by removing peers if the connection becomes disconnected, and timeouts/useless responses. This still happens quite frequently.

TODO - test this PR out on a mainnet node
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 03:11:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6209" class=".btn">#6209</a>
            </td>
            <td>
                <b>
                    worldstate refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

for verkle, I’m starting a refactor. In simple terms, many classes can distinguish whether they’re in ‘bonsai’ or ‘forest’ mode, so a generic interface doesn’t offer much value, except for some minor and synchronization parts.
So, I’ve developed a ’WorldstatestorageCoordinator class. This will have a storage strategy, which could be either ‘bonsai’ or ‘forest’. This coordinator is needed when we’re unsure about the storage mode we use, and it helps for the routing process. when we’re sure about the storage mode, we directly use the appropriate strategy.
This approach reduces the number of generic interfaces, eliminating locations that are not applicable to modes like ‘forest’ or other not clean things like that.
Will be better when we will have to add some custom method or field for verkle

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 10:14:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6207" class=".btn">#6207</a>
            </td>
            <td>
                <b>
                    moved some logs to trace level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span><span class="chip">logging</span><span class="chip">ux</span>
            </td>
            <td>
                * move "Requesting x headers" etc to trace level logging
* use peer.shortNodeId rather than logging the whole peer record
* move "Wrote initial crypto handshake message" to trace
* also a couple of frequently logged tx pool logs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 02:20:03 +0000 UTC
    </div>
</div>

