---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/302" class=".btn">#302</a>
            </td>
            <td>
                <b>
                    Separate tx validation from block processor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In preparation for implementing config-tx validation pre-order (future commit), we separate the tx-validation logic into a separate package.
    - All validation code was moved to a new package
    - Respective types & methods used in other packages made Public (e.g. ValidateBlock)
    - The block processor consumes a single method during commit: 'ValidateBlock'.
    - Generation of Validator extracted from inside the block processor, now in transaction processor
    - Validator now can be shared with other components (future commit)
    
The block processor consumes a single method during commit: 'ValidateBlock'.
    
This will make it easier to expose validation logic to pre-ordering components.
    
This commit presents **no functional change**, just refactoring of existing code.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 13:30:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/301" class=".btn">#301</a>
            </td>
            <td>
                <b>
                    Validate genesis block: code hygiene
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Eliminate some code duplication when validating the genesis block (block number 1).
No functional change.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 13:28:37 +0000 UTC
    </div>
</div>

