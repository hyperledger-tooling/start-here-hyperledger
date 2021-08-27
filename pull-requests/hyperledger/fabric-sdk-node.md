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

