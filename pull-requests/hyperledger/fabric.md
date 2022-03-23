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
                PR <a href="https://github.com/hyperledger/fabric/pull/3296" class=".btn">#3296</a>
            </td>
            <td>
                <b>
                    Add Discord chat to Fabric docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Replace RocketChat references with Discord in Fabric docs.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 20:56:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3295" class=".btn">#3295</a>
            </td>
            <td>
                <b>
                    fix unittest failure (#3294)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shivdeep Singh <Shivdeep.Singh@ibm.com>

#### Type of change

- Bug fix
- Test update

#### Description

Unittest __snapshot on accumlated bytes condition met__ in `orderer/consensus/etcdraft` was failing due to *Expect* conditions not met. Replaced *Expect* condition with *Eventually* which waits for some time to check for expected condition. 

#### Related issues
- [3294](https://github.com/hyperledger/fabric/issues/3294)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 05:08:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3292" class=".btn">#3292</a>
            </td>
            <td>
                <b>
                    Change membership documentation about public keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Documentation update
#### Description
> a mechanism is required to enable that proof which is where the MSP comes in

Identity can be proven just by signing the transaction and verifying with the public key on the certificate, proving identity is not where the MSP comes in, this is more related to how CAs issue the key-pair.

> The private key is used to produce a signature on a transaction that only the corresponding public key, that is part of an MSP, can match.

The sentence does not say anything about whether this public key matches invalid signatures, it only says that given that particular signature, only that particular public key can match. It should go along the lines of "only a valid signature will work". The sentence has been removed as I have adapted the paragraph.

I do not have experience with Fabric; these changes are based off my reading of the documentation. Am I right to assume that the member's public keys do not need to be added to the organization's MSP in the current version? Please correct me if I am wrong. Thank you.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-19 13:58:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3289" class=".btn">#3289</a>
            </td>
            <td>
                <b>
                    Locate correct block number for transaction ID in ChaincodeEvents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the request contains an `after_transaction_id`, start reading from the block containing that transaction ID and ignore any specified start block. If the specified transaction has not been committed in a block, fall back to any specified start block or next committed block.

Enhancement requested in review of PR #3283
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 14:33:19 +0000 UTC
    </div>
</div>

