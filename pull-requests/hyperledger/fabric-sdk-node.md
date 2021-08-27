---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/493" class=".btn">#493</a>
            </td>
            <td>
                <b>
                    Fix build break (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of relevant parts of f1378ab7a08f07c29813cd572c0d88defbab8808 from main branch.

New TypeScript release caused compile / lint failures.

- Pinned to a more specific TypeScript version
- Minor type and lint changes

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 17:44:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/492" class=".btn">#492</a>
            </td>
            <td>
                <b>
                    Resolve build error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 17:27:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/491" class=".btn">#491</a>
            </td>
            <td>
                <b>
                    Fix build break
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                New TypeScript release caused compile / lint failures.

- Pinned to a more specific TypeScript version
- Minor type and lint changes
- Some additional exclusions to license check to avoid failures in development environment

Signed-off-by: Mark S. Lewis <mark_lewis@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 17:13:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/490" class=".btn">#490</a>
            </td>
            <td>
                <b>
                    FABN-1530: Timestamp added to full and private block transaction events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 15:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/489" class=".btn">#489</a>
            </td>
            <td>
                <b>
                    add: more clear exception log error for no peers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # What does this PR do?

- Raises an exception if there are no endorsing peers in SingleQueryHandler peers list with a more informative error log;

# Why does it is relevant?

The evaluation method works like the presented fluxogram:

![image](https://user-images.githubusercontent.com/6313981/131119231-e2732f3f-505e-42b1-aa05-8e42ea1b972f.png)

By throwing an exception that doesn't inform the reason for the error (by presenting an empty error list), it may cause problems for developers to understand what it have to do in order to fix it.

Here is a some stackoverflow entries of users confused about this error:

- [SOUPTIK BANERJEE](https://stackoverflow.com/questions/66316846/singlequeryhandler-evaluate-message-query-failed-errors-stack-fabricer)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-27 11:21:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/488" class=".btn">#488</a>
            </td>
            <td>
                <b>
                    Revert back release 2.2.9 changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-25 09:24:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    Release PR for version 2.2.9 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sapthasurendran <saptha.surendran@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-24 19:03:16 +0000 UTC
    </div>
</div>

