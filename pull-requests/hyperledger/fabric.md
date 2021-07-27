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
                PR <a href="https://github.com/hyperledger/fabric/pull/2784" class=".btn">#2784</a>
            </td>
            <td>
                <b>
                    FAB-18067 Discovery support Implicit Collections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implemented the fix as suggested by Yacov in his Jira comment.

Verified the fix works against the asset-transfer-secured-agreement sample which uses implicit collections.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 12:21:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2783" class=".btn">#2783</a>
            </td>
            <td>
                <b>
                    Update to latest major version of Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Brett Logan <lindluni@github.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-24 23:40:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2780" class=".btn">#2780</a>
            </td>
            <td>
                <b>
                    FAB 18365 IT flake evictionsuspector failed to read eviction 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Description
In failing case, the OSN being removed has committed the config change but failed to receive apply_config msg to halt the chain. This state is defined to be handled as part of the eviction suspicion logic. But it failed when evictionsuspector failed to check from lastconfig block if chain is up-to-date. 

Fix: Updated the order of statements which looks at the latest config block and block height validation.

#### Type of change
- Bug fix

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 11:02:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2779" class=".btn">#2779</a>
            </td>
            <td>
                <b>
                    Hardening raft catchup IT
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
        Created At 2021-07-22 23:42:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2778" class=".btn">#2778</a>
            </td>
            <td>
                <b>
                    Merge and enhance coding guidelines across github and wiki
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enhances and merges the additional coding guidelines present in the [wiki page](https://wiki.hyperledger.org/display/fabric/Coding+Guidelines) into the coding guidelines page maintained in the docs at github.

Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 22:43:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2776" class=".btn">#2776</a>
            </td>
            <td>
                <b>
                    Update private data docs - remove SDK reference (backport #2770)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2770 done by [Mergify](https://mergify.io).


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
        Created At 2021-07-22 17:34:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2775" class=".btn">#2775</a>
            </td>
            <td>
                <b>
                    Additional documentation for implicit private data collections (backport #2772)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2772 done by [Mergify](https://mergify.io).


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
        Created At 2021-07-22 16:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2774" class=".btn">#2774</a>
            </td>
            <td>
                <b>
                    Additional documentation for implicit private data collections (backport #2772)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2772 done by [Mergify](https://mergify.io).


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
        Created At 2021-07-22 16:17:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2773" class=".btn">#2773</a>
            </td>
            <td>
                <b>
                    FABGW-25 Endorse using generated ChaincodeInterest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change the Endorse() method logic as described in the design document attached to the Jira.
- Process proposal on local org peer.
- Using the ChaincodeInterest in the propsal response, invoke discovery to obtain a layout that contains the local org
- Obtain the remaining endorsements
- Build the transaction to send back to the client.

Extra unit tests added to test the new logic.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 13:07:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2772" class=".btn">#2772</a>
            </td>
            <td>
                <b>
                    Additional documentation for implicit private data collections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                Add additional documentation for implicit private data collections.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 11:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2771" class=".btn">#2771</a>
            </td>
            <td>
                <b>
                    FABGW-25 Test for system chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit addresses the closing comments in PR #2767:

- Skip systems chaincode in this block as well
- Add a test that asserts that the system chaincodes are indeed skipped

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 08:59:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2770" class=".btn">#2770</a>
            </td>
            <td>
                <b>
                    Update private data docs - remove SDK reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove reference to SDK since SDK is no longer used to deploy chaincode.
Also remove reference to legacy lifecycle (legacy lifecycle
remains fully documented in release-1.4 docs and in the main branch CLI reference doc).

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 23:09:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2769" class=".btn">#2769</a>
            </td>
            <td>
                <b>
                    [FAB-11334] Adds a function to purge a ledger's transient storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                #### Type of change

- New feature

#### Description

This introduces a transientstore.Delete(ledgerID) routine to assist with the bookkeeping while unjoining a peer from a channel.  Before removing the transient storage, the store is marked as UNDER_DELETION in a system leveldb, providing an opportunity to recover from a failed deletion at the next peer initialization.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Additional details

#### Related issues

- [FAB-11334](https://jira.hyperledger.org/browse/FAB-11334)

Resolves #2786 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 16:49:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2768" class=".btn">#2768</a>
            </td>
            <td>
                <b>
                    [FAB-18527] Discovery supports DisregardNamespacePolicy hint from client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds support for a boolean flag in the chaincode call: DisregardNamespacePolicy
Its role is to hint to discovery that the client wishes to ask about endorsement policies
of either state based endorsement policies of given keys, or of collection endorsement policies
that exist for given collection names.

In case no state based endorsement policies are given in the bespoken chaincode call,
and also no collection level endorsement policies of the given collection names are found,
specifying the DisregardNamespacePolicy hint for that chaincode call will result in an error,
as there is no endorsement policy to compute on.

Change-Id: I299afd40063a0cf1cee34d6034eaa02fe6fc6707
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 12:37:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2767" class=".btn">#2767</a>
            </td>
            <td>
                <b>
                    FABGW-25 Build ChaincodeInterest in TX simulator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                During transaction simulation, capture extra information to build a ChaincodeInterest structure specific to the chaincode invocation as follows:
- Which private data collections are read from.
- The SBE policies associated with any states that a written to.

Following simulations, the ChaincodeInterest structure is built and returned in the ProposalResponse message.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 11:07:09 +0000 UTC
    </div>
</div>

