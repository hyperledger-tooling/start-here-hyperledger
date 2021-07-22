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
                
            </td>
            <td>
                #### Type of change

- New feature

#### Description

This introduces a transientstore.Delete(ledgerID) routine to assist with the bookkeeping while unjoining a peer from a channel.  Before removing the transient storage, the store is marked as UNDER_DELETION in a system leveldb, providing an opportunity to recover from a failed deletion at the next peer initialization.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Additional details

*This is a DRAFT PR - NOT READY FOR MERGE*

Discussion points for review: 
- The original design was to store the set of ledgers/transient storage under deletion as a proto message structure in the system leveldb.  In this implementation the storage array under deletion is written as a json array in the leveldb.  I am open to moving this over to a proto message.
- This PR needs some additional test cases. 
- There may be some lingering issues with db handles, providers, leveldb helpers, etc. getting closed correctly.  When reviewing this PR, please note the handling of open/close for the providers and comment on the approach in this change.
- `StoreProvider` is an interface covering a subset of the functions received by the `storeProvider`.  The routines to track the deletion status are received by the `storeProvider`, but could also be scoped to the package and accept the provider argument as a function parameter.   There are a couple of golang _Type Assertions_ in the test routines, which is OK but it feels like this module can / should be refactored (not in this PR) to clean up the overall API design. 

#### Related issues

- [FAB-11334](https://jira.hyperledger.org/browse/FAB-11334)


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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2764" class=".btn">#2764</a>
            </td>
            <td>
                <b>
                     [FAB-18527] Discovery supports state based endorsement queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds support for state based endorsement queries to the discovery service.
    
When state based endorsement policies are passed in the chaincode call,
discovery now combines them and then requires their combinations to be satisfied as well
as the chaincode endorsement policies.
    
Support for chaincode calls with *only* state based endorsement is future work and not implemented
yet because of lack of a way to express this intent in the protobuf definition.
    
Change-Id: I005a6abca77061cd531888cdff544691b25d09ec
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-17 23:05:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2763" class=".btn">#2763</a>
            </td>
            <td>
                <b>
                    [FABGW-25] Move chaincode interest to proposal response proto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit picks up the changes in pull request https://github.com/hyperledger/fabric-protos/pull/59 which entail:

- Moving chaincode interest to proposal response
- Adding a policy for state based endorsement in the chaincode call in preperation for FABGW-25

Change-Id: Ia0a0d57964daad9c773135d2e6c1d3a96e4df079
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-17 23:04:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2762" class=".btn">#2762</a>
            </td>
            <td>
                <b>
                    [FAB-18521] Replicate block metadata with block while OSN catching up
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While OSN catches up replicating block from the up-to-date replica, the metadata information omitted, i.e.

``
c.support.WriteBlock(block, nil)
``

Where `nil` substitutes for block's metadata. In this commit, the consenters metadata extracted from the replicated
block and is written with the block.

Signed-off-by: Artem Barger <artem@bargr.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-17 22:01:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2761" class=".btn">#2761</a>
            </td>
            <td>
                <b>
                    [FAB-18521] Fixing flaky IT, send remove tx to another node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                PR #2748, introduced new IT to ensure the fix. However, there is some flakiness manifested with this IT, caused by sending the remove consenter transaction to the "to be removed" node. Removing the consenter is a config transaction where codes after sending it ensure a new block with the config update successfully committed, which is the root cause for the flakiness. Once OSN is removed from the channel, it no longer can server deliver requests for clients trying to fetch from it.

This commit, fixes it by sending remove OSN config updated transaction
to a different node instead.

Signed-off-by: Artem Barger <artem@bargr.net>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 23:18:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2760" class=".btn">#2760</a>
            </td>
            <td>
                <b>
                    Output File Exists Error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->


- Improvement (improvement to code, performance, etc)
- Test update

#### Description

- Compare tool no longer overwrites existing files and will throw an error instead. Compare function now takes in the output directory instead of the output file as an argument.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 23:15:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2759" class=".btn">#2759</a>
            </td>
            <td>
                <b>
                    Update CHANGELOG.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update CHANGELOG.md to indicate that the changelog is now maintained in GitHub.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 18:17:10 +0000 UTC
    </div>
</div>

