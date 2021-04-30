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
                PR <a href="https://github.com/hyperledger/fabric/pull/2574" class=".btn">#2574</a>
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
        Created At 2021-04-30 06:47:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2573" class=".btn">#2573</a>
            </td>
            <td>
                <b>
                    Feature/fix trouble with pkcs11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Fix troubles with PKCS11

#### Type of change

- Bug fix

#### Description

Simple changes that fix these errors on 1.4 Path:
- When setting ORDERER_GENERAL_BCCSP_PKCS11_SECURITY orderer variable the orderer fails saying that the security value is a string and not an int.
- When running `GO_TAGS=pkcs11 make docker` the fabric-tools docker image doesn't include a PKCS11 provider.

#### Related issues

https://jira.hyperledger.org/browse/FAB-18457


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 20:36:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2572" class=".btn">#2572</a>
            </td>
            <td>
                <b>
                    Fix incorrect error message in Gateway submit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As pointed out in previous PR review, the error message was incorrect when the gateway can’t connect to the BroadcastClient. (https://github.com/hyperledger/fabric/pull/2508#discussion_r601777021)

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 10:50:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2570" class=".btn">#2570</a>
            </td>
            <td>
                <b>
                    FABGW-19: Secure CommitStatus service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 16:10:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2569" class=".btn">#2569</a>
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
        Created At 2021-04-28 06:15:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2568" class=".btn">#2568</a>
            </td>
            <td>
                <b>
                    Corrected function name in comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sukill <ckdrms622@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 06:58:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2567" class=".btn">#2567</a>
            </td>
            <td>
                <b>
                    Add log warning for unathorized operations requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It is not obvious which operations requests require a client cert to be passed
when TLS is enabled on a peer but clientAuthRequired is not enabled.
This new log warning message will help troubleshoot failed connections to operations services
when a client cert is not passed.

Docs are also updated to clarify client cert requirements.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 19:46:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2566" class=".btn">#2566</a>
            </td>
            <td>
                <b>
                    Removed early mentioning of organization R3 (backport #2542)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2542 done by [Mergify](https://mergify.io).

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
        Created At 2021-04-26 19:15:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2564" class=".btn">#2564</a>
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
        Created At 2021-04-25 02:36:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2563" class=".btn">#2563</a>
            </td>
            <td>
                <b>
                    Updates in main branch for release v2.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and script for v2.3.2.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 21:49:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2562" class=".btn">#2562</a>
            </td>
            <td>
                <b>
                    v2.3.2 release commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates doc and release notes for v2.3.2.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 17:21:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2561" class=".btn">#2561</a>
            </td>
            <td>
                <b>
                    v2.2.3 release commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates docs and release notes for v2.2.3.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 17:09:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2560" class=".btn">#2560</a>
            </td>
            <td>
                <b>
                    v1.4.12 release commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates docs and release notes for v1.4.12.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 16:51:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2559" class=".btn">#2559</a>
            </td>
            <td>
                <b>
                    Add debug for policy defaults
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When troubleshooting issues, it is helpful to know which policy is
applied for resource requests.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 16:28:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2558" class=".btn">#2558</a>
            </td>
            <td>
                <b>
                    Remove redundant casts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit removes redundant casts in discovery/service.go
    
Change-Id: I6b52ba91ccbe0ffeb696943aafa12fa3e07012fd
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 16:02:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2557" class=".btn">#2557</a>
            </td>
            <td>
                <b>
                    Remove redundant comma
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit removes a redundant comma in an error log message in discovery/service.go
    
Change-Id: I1daaf673d942ee7a44eefcb62316e5807f10bcc6
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 16:01:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2556" class=".btn">#2556</a>
            </td>
            <td>
                <b>
                    Remove redundant type cast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit removes a redundant type cast in gossip/comm/comm_impl.go

Change-Id: Ie8b921a5097f0d05f6645e67c31940c9daec0eb5
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 15:54:42 +0000 UTC
    </div>
</div>

