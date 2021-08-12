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
                PR <a href="https://github.com/hyperledger/fabric/pull/2833" class=".btn">#2833</a>
            </td>
            <td>
                <b>
                    fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wuqiaomin <wuqiaomin2@huawei.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 09:03:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2832" class=".btn">#2832</a>
            </td>
            <td>
                <b>
                    Add release notes for v2.4.0-beta release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add release notes for v2.4.0-beta release.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 01:18:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2830" class=".btn">#2830</a>
            </td>
            <td>
                <b>
                    Fix small doc errors (backport #2816)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span><span class="chip">doc-merge</span>
            </td>
            <td>
                This is an automatic backport of pull request #2816 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 18:28:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2829" class=".btn">#2829</a>
            </td>
            <td>
                <b>
                    Better error messages from Gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Include some of the detail information in the top level gRPC error message to aid problem determination for client applications.

Resolves #2806
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 16:04:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2828" class=".btn">#2828</a>
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

Signed-off-by: sardChen <sard.chen@gmail.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 14:42:06 +0000 UTC
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

