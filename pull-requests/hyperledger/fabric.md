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
                PR <a href="https://github.com/hyperledger/fabric/pull/2632" class=".btn">#2632</a>
            </td>
            <td>
                <b>
                    Pass go tags to tools container (bp #2136) 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

Backport to version 1.4 to fix trouble: when running GO_TAGS=pkcs11 make docker, the fabric-tools docker image doesn't include a PKCS11 provider.

#### Related issues

https://lists.hyperledger.org/g/fabric/topic/error_using_hsm_in_fabric/78302231?p=
https://github.com/hyperledger/fabric/pull/2136
[FAB-18457](https://jira.hyperledger.org/browse/FAB-18457)
https://github.com/hyperledger/fabric/pull/2573
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 01:47:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2631" class=".btn">#2631</a>
            </td>
            <td>
                <b>
                    [FAB-17900] Fixes numeric env variable override bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description

Backport fix for version 1.4 for error: when setting ORDERER_GENERAL_BCCSP_PKCS11_SECURITY orderer variable, the orderer fails saying that the security value is a string and not an int.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

[FAB-17900](https://jira.hyperledger.org/browse/FAB-17900)
[FAB-18457](https://jira.hyperledger.org/browse/FAB-18457)
https://github.com/hyperledger/fabric/pull/2573
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 01:25:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2630" class=".btn">#2630</a>
            </td>
            <td>
                <b>
                    Fix minor code comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Improvement

#### Additional details
Address [comment](https://github.com/hyperledger/fabric/pull/2614#discussion_r642961892) in previous PR

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 15:46:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2626" class=".btn">#2626</a>
            </td>
            <td>
                <b>
                    [FAB-18479] Log error if orderer can't forward SubmitRequest (backport #2624)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2624 done by [Mergify](https://mergify.io).


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
        Created At 2021-05-31 11:51:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2625" class=".btn">#2625</a>
            </td>
            <td>
                <b>
                    [FAB-18479] Log error if orderer can't forward SubmitRequest (backport #2624)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2624 done by [Mergify](https://mergify.io).


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
        Created At 2021-05-31 11:51:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2624" class=".btn">#2624</a>
            </td>
            <td>
                <b>
                    [FAB-18479] Log error if orderer can't forward SubmitRequest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [FAB-18479] Log error if orderer can't forward SubmitRequest to Raft leader

If order cannot forward client transaction SubmitRequest to Raft leader,
it only logged it in a debug message. And since the error does
not get returned to the client either, it is difficult to identify
and troubleshoot.

This commit changes the message to an error in the orderer log.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-30 19:32:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2621" class=".btn">#2621</a>
            </td>
            <td>
                <b>
                    fix duplicate entry in code snippet (backport #2616)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2616 done by [Mergify](https://mergify.io).


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
        Created At 2021-05-29 02:37:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2618" class=".btn">#2618</a>
            </td>
            <td>
                <b>
                    fix duplicate entry in code snippet (backport #2616)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2616 done by [Mergify](https://mergify.io).


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
        Created At 2021-05-29 02:35:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2616" class=".btn">#2616</a>
            </td>
            <td>
                <b>
                    fix duplicate entry in code snippet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Gabriel <chris_gabriel_98@yahoo.com>

Code snippet had duplicate export.

#### Type of change

- Documentation update

#### Description

Fix duplicate export entry in code snippet.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 22:32:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2615" class=".btn">#2615</a>
            </td>
            <td>
                <b>
                    Update Building docs to reflect UI changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the Building on GitHub instructions
to reflect UI changes in readthedocs.org

Signed-off-by: Asher T. Scott <ashertlalka@gmail.com>
Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 21:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2614" class=".btn">#2614</a>
            </td>
            <td>
                <b>
                    Add block-number along with validation code for a given TXID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
This allows gateway to pass on additional relevant info to client and for using it for logging that could be helpful in debugging
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 17:26:13 +0000 UTC
    </div>
</div>

