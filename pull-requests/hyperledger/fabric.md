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
                PR <a href="https://github.com/hyperledger/fabric/pull/3047" class=".btn">#3047</a>
            </td>
            <td>
                <b>
                    Updates to Gateway doc topic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update to Fabric Gateway doc topic.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 04:28:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3045" class=".btn">#3045</a>
            </td>
            <td>
                <b>
                    Enhance gateway error logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add logic to determine the origin of the error returned by ProcessProposal, and whether the evaluate/endorse methods should close the connection to the peer and/or retry the proposal on another peer.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 16:33:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3044" class=".btn">#3044</a>
            </td>
            <td>
                <b>
                    Clarify ProcessProposal error handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add comments to clarify ProcessProposal error handling intent.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-13 16:09:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3042" class=".btn">#3042</a>
            </td>
            <td>
                <b>
                    Gateway overview edited
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

New Fabric Gateway overview doc, written by @andrew-coleman, reviewed by @denyeart, and edited by @joshhus. 

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature
- Documentation update

#### Description

Fabric Gateway simplifies client app / SDK development by migrating transaction endorsement functionality to a Fabric Gateway peer. 

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

Some related doc file reviews and edits are still TBA.

#### Related issues

https://github.com/hyperledger/fabric/issues/2807

#### Release Note

Fabric Gateway simplifies client application development by migrating transaction endorsement functionality from the client to the Fabric Gateway peer. This new gateway functionality is currently optional. Simplified SDKs are provided for clients who choose to implement the new gateway. Read more at (link to documentation start -- gateway.md). 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 21:12:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3040" class=".btn">#3040</a>
            </td>
            <td>
                <b>
                    Facilitate unaware threshold signature endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit contains the following two seemingly unrelated changes, each on its own preserving current Fabric behavior:

1. **Deduplicate endorsements in createTx**
This commit makes createTx de-duplicate endorsers according to their identity.
Meaning, when multiple but identical endorsements (same identity) are passed to
the createTx function, it returns a transaction with unique endorsements, and without repeated endorsers.
Since at validation, endorsers are anyway de-duplicated, this commit preserves current system behavior.

2. **Support identity based endorsement policy in discovery**
Currently, whenever a chaincode's endorsement policy contains an identity principal, discovery rejects the policy,
saying that it contains a principal it does not support. This commit simply makes discovery classify the principal.


**Making clients and gateways unaware of a threshold signature scheme**
This commit enables advanced use cases, in which case the endorsements collected for transaction
submission contain identical identities that represent a threshold or aggregation signature scheme.

In such a case, peers can be deployed with custom endorsement plugins and generate a threshold/aggregation signature,
but the flow of service discovery, the client, and peer gateway remains the same.

The endorsement policy can to be an OR over two mutually exclusive cases:
1. An AND over a set of organizational principals (such as Org1.Peer and Org2.Peer)
2. An OR over one or more identities (which can only be signed in collaboration among the peers)
Discovery will always return only combinations of the former kind since no peer can identify with an identity of the latter kind.

The flow will then be as follows: 
1. The client and the gateway interact as usual, and the gateway collects endorsements from several peers.
2. The peers, using the endorsement plugin, engage in a protocol at which end they all return the same endorsement.
3. The gateway submits the transaction (this time, with a single endorsement) to the orderer.
4. Upon transaction validation we validate a single endorsement instead of several.

By enabling threshold signatures, we can maintain security (multiple organizations execute the smart contract and sign over the execution results) without sacrificing performance (transaction ends up with having a single endorsement)

Change-Id: I9193187ae6b08791f8762a9d325442d156c4f828
Signed-off-by: Yacov Manevich <yacovm@il.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 14:03:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3038" class=".btn">#3038</a>
            </td>
            <td>
                <b>
                    Reword evaluate() error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When no suitable peers are available to evaluate a transaction, the registry returns an error.  The message should be reworded to make clear it is being used for evaluation rather than endorsement.

Resolves https://github.com/hyperledger/fabric-gateway/issues/282

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-10 13:17:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3037" class=".btn">#3037</a>
            </td>
            <td>
                <b>
                    no gateway via cli - tutorials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

The new Fabric Gateway peer function is being documented, but the CLI cannot yet access the gateway peer. So these tutorials which call the `peer chaincode invoke` command need a mention of the requirement to still specify all endorsement peers. 

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

https://github.com/hyperledger/fabric/issues/2807

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 21:33:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3036" class=".btn">#3036</a>
            </td>
            <td>
                <b>
                    Add extra info to error message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When processing an endorsement plan, failure to connect to remote peers could lead to an error saying there aren’t enough endorsers to satisfy the policy.  This commit add the list of peers that failed to commit.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 17:48:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3032" class=".btn">#3032</a>
            </td>
            <td>
                <b>
                    Use correct timeout option
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The gateway’s endpoint connection factory is currently using the EndorsementTimeout option when making connections.  It should be using the DialTimeout.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-09 13:34:17 +0000 UTC
    </div>
</div>

