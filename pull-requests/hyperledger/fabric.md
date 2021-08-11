---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2824" class=".btn">#2824</a>
            </td>
            <td>
                <b>
                    Fix FAB-18528: remove panic in ifConfig func
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix issues: FAB-18528. When received the constructed message from the malicious node (through the interface "chain.rpc.SendSubmit(dest uint64, request *orderer.SubmitRequest, report func(err error))"), all orderers will breakdown immediately.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 10:30:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2822" class=".btn">#2822</a>
            </td>
            <td>
                <b>
                    Add slash command for invalid issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a "/invalid" command that when typed in an issue will let users know the purpose of GitHub issues and close the issue.

This can be used when a user opens an issue seeking help, rather than to report a bug or request a feature. Simply typing `/invalid` will reply to the issue with the below comment and automatically close the issue:

```
Thank you for opening this issue.

GitHub Issues is a tool for tracking bugs, feature requests, and work in general that 
relates directly to the Fabric codebase. It is not for general help requests. Please 
use one of the following forums to request help for your issue:

- RocketChat: https://chat.hyperledger.org
- Fabric Mailing List: fabric@lists.hyperledger.org
```

Signed-off-by: Brett Logan <lindluni@github.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 19:06:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2816" class=".btn">#2816</a>
            </td>
            <td>
                <b>
                    Fix small doc errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Arnaud J Le Hors <lehors@us.ibm.com>

#### Type of change

- Documentation update

#### Description

Fixes a couple of small errors (typo like)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 17:04:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2805" class=".btn">#2805</a>
            </td>
            <td>
                <b>
                    Options for GRPC message size configurable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement 

#### Description
- Configurable options to update GRPC max message size.  Options added both in peer and orderer node configuration.

#### Related issues
- #2804 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 18:19:19 +0000 UTC
    </div>
</div>

