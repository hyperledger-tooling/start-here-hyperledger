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
                PR <a href="https://github.com/hyperledger/besu/pull/4869" class=".btn">#4869</a>
            </td>
            <td>
                <b>
                    Remove Deprecated Networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Remove the Ropsten, Kiln, Shandong, and Astor network definitions from the built-in network list.  Includes tendrils depending on and testing such configurations.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-30 18:17:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4868" class=".btn">#4868</a>
            </td>
            <td>
                <b>
                    Enable EOF in Shanghai
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

Enable EOF into shanghai by wiring it into protocol specs.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-30 16:32:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4867" class=".btn">#4867</a>
            </td>
            <td>
                <b>
                    [Work in Progress] Attempt to fix CPU spikes issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
This PR is an attempt to fix CPU spikes issue (#4838).
A CPU profiling on a synced node showed that most of the time is spent on calculating peer outstanding requests. This is triggered by attemptExecution called for each pending request by reattemptPendingPeerRequests and triggered by either EthPeers.dispatchMessage or EthPeers.disconnect.

EthPeers.dispatchMessage
&nbsp;&nbsp;&nbsp;&nbsp;reattemptPendingPeerRequests
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;attemptExecution
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hasAvailableRequestCapacity
       
EthPeers.registerDisconnect
&nbsp;&nbsp;&nbsp;&nbsp;reattemptPendingPeerRequests
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;attemptExecution
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;hasAvailableRequestCapacity

So each time, a message is dispatched or a peer is disconnected, Besu will iterate over all the pending requests and try to find an available peer for each single request. 
 
<img width="1704" alt="image" src="https://user-images.githubusercontent.com/5099602/209989962-0295288c-c125-4653-a177-90d7bb0fa843.png">

By looking to the size of pending requests, we can see that this can be huge (more than 200k), and there is a clear correlation with the CPU spikes. My understanding here is that Besu node is spammed sometimes by huge amount of requests which results of a lot of pending requests.

![image](https://user-images.githubusercontent.com/5099602/209990873-cb0c9b54-8666-44e1-9de2-66097e81341a.png)

The idea behind this PR is to avoid unnecessary computation and iterate over available peers instead of iterating over pending requests.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Should fix #4838

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-29 18:26:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4866" class=".btn">#4866</a>
            </td>
            <td>
                <b>
                    Do not apply final arguments ErrorProne to generated code
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

Custom ErrorProne checks should not be validating generated code we cannot change, hence the "method params must be final" ErrorProne check will not fire in classes with a "generated" annotation.  This covers Dagger generated code.

Signed-off-by: Danno Ferrin <danno.ferrin@swirldslabs.com>

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [X] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-28 15:37:57 +0000 UTC
    </div>
</div>

