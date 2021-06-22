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
                PR <a href="https://github.com/hyperledger/fabric/pull/2701" class=".btn">#2701</a>
            </td>
            <td>
                <b>
                    Mandate TLS 1.2 or higher in fabhttp package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit ensures that the HTTP server that is spawned by the fabhttp package
only accepts TLS handshakes from clients that attempt to use TLS 1.2 or higher.

Change-Id: Ia25482d9c96f68506724a58258451311b3d63208
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 20:06:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2699" class=".btn">#2699</a>
            </td>
            <td>
                <b>
                    [FAB-18485]Fabric orderer - add config option for client keepalives
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added config option for orderer client keepalives.  Defaults defined as per the
existing hard coded values. 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 10:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2698" class=".btn">#2698</a>
            </td>
            <td>
                <b>
                    Address PR comments in Gateway integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 09:29:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2697" class=".btn">#2697</a>
            </td>
            <td>
                <b>
                    Fix two typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Eyers <dme@cs.otago.ac.nz>

Fixed two minor typographical errors in the documentation.

#### Type of change

- Documentation update

#### Description

Fixed two minor typographical errors in the documentation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 04:19:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2695" class=".btn">#2695</a>
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
        Created At 2021-06-21 02:53:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2693" class=".btn">#2693</a>
            </td>
            <td>
                <b>
                    Retire Brett Logan as maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's time, those who are active with the project should maintain it, which is no longer me unfortunately, I wish everyone the best in the future and thank you for everything everyone has done for me.

I've removed my access to all Hyperledger resources.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 14:28:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2692" class=".btn">#2692</a>
            </td>
            <td>
                <b>
                    Cherry pick deploy CC fixes into release-2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

#### Type of change

- Bug fix
- Documentation update

#### Description

Cherry pick updates that were made to the deploy CC tutorial in the release-2.2 branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 12:46:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2691" class=".btn">#2691</a>
            </td>
            <td>
                <b>
                    Cherry pick deploy CC fixes to main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

#### Type of change

- Bug fix
- Documentation update

#### Description

Cherry pick fixes made to the deploy CC topic to the main branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 12:36:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2690" class=".btn">#2690</a>
            </td>
            <td>
                <b>
                    Handle missing endpoints from discovery
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For some reason the discovery PeersOfChannel function does not
return an endpoint for the local peer, which the gateway was
relying on

Rather than updating PeersOfChannel to return the endpoint when
there is one, to match the Peers function, this change updates
how the gateway identifies the local peer

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 11:23:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2689" class=".btn">#2689</a>
            </td>
            <td>
                <b>
                    Clarify orderers seeing the transaction data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Having the answer start with a `No` is misleading. Beginners
who generally rely on FAQ section to understand the fundamentals
thought that orderers do not receive any information about a
transaction.

With the explanation on what is available with orderers clarifies
the intent served in this FAQ. i.e. Orderers do get the
transaction but at their goodwill they will not open the
transaction, as they do not have a need to open them.

#### Additional details

NA, documentation update

#### Related issues

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 09:04:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2688" class=".btn">#2688</a>
            </td>
            <td>
                <b>
                    Clarify "identity expired" error messages (#2685)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Peer and Orderer have several "identity expired" error messages.
Clarify error messages to indicate which identity has expired.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 20:25:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2686" class=".btn">#2686</a>
            </td>
            <td>
                <b>
                    Clarify "identity expired" error messages (backport #2685)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2685 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-15 20:11:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2685" class=".btn">#2685</a>
            </td>
            <td>
                <b>
                    Clarify "identity expired" error messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Peer and Orderer have several "identity expired" error messages.
Clarify error messages to indicate which identity has expired.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 15:09:24 +0000 UTC
    </div>
</div>

