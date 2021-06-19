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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2683" class=".btn">#2683</a>
            </td>
            <td>
                <b>
                    Fix spelling mistakes in the Github Contributions page (backport #2679)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2679 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-14 18:00:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2682" class=".btn">#2682</a>
            </td>
            <td>
                <b>
                    Fix spelling mistakes in the Github Contributions page (backport #2679)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2679 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-14 18:00:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2681" class=".btn">#2681</a>
            </td>
            <td>
                <b>
                    Fix spelling mistakes in the Github Contributions page (backport #2679)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2679 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-14 17:59:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2680" class=".btn">#2680</a>
            </td>
            <td>
                <b>
                    Fix spelling mistakes in the Github Contributions page (backport #2679)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span><span class="chip">docs</span>
            </td>
            <td>
                This is an automatic backport of pull request #2679 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-14 17:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2679" class=".btn">#2679</a>
            </td>
            <td>
                <b>
                    Fix spelling mistakes in the Github Contributions page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

#### Type of change

- Bug fix
- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 16:18:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2678" class=".btn">#2678</a>
            </td>
            <td>
                <b>
                    [FAB-18493] Fix broken links in release-1.4 docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>


#### Type of change

- Bug fix
- Documentation update

#### Description

Fix broken links found by link checker in release-1.4 docs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 16:03:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2677" class=".btn">#2677</a>
            </td>
            <td>
                <b>
                    [FAB-18492] Fix broken links in the 2.0 release docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                Signed-off-by: Nikhil Gupta <ngupta@symbridge.com>

#### Type of change

- Bug fix
- Documentation update

#### Description

Fix broken links found by link report in 2.0 docs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 15:34:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2676" class=".btn">#2676</a>
            </td>
            <td>
                <b>
                    [FAB-18489] fix links in 2.1 release docs
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

Fix links detected by the link checker in the release-2.1 docs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 14:37:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2675" class=".btn">#2675</a>
            </td>
            <td>
                <b>
                    [FAB-18484] Return transaction forwarding result back to the client synchronously (backport #2666)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit makes a Raft follower wait for the transaction forwarded to the leader to be sent into
the gRPC stream, and returns the result (success or failure) back to the client accordingly.

Before this commmit, the behavior was that it returns success after enqueueing it into the message queue,
which might have resulted in the transaction being dropped but a success being returned to the client.

Change-Id: I0cd45540be4988845663eb0c68f76fed2ff25b94
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-13 22:28:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2672" class=".btn">#2672</a>
            </td>
            <td>
                <b>
                    [FAB-18484] Return transaction forwarding result back to the client synchronously (backport #2666)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2666 done by [Mergify](https://mergify.io).


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
        Created At 2021-06-13 21:57:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2671" class=".btn">#2671</a>
            </td>
            <td>
                <b>
                    Update email address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updating my email address to the active one. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-13 20:21:34 +0000 UTC
    </div>
</div>

