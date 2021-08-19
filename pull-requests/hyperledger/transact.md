---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    Add feature deps for family-command-workload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the feature `"family-command-workload"` such that compiling like:

```
$ cargo check --manifest-path libtransact/Cargo.toml --features family-command-workload
```

will successfully compile.

It also makes the indenting consistent in the Cargo.toml
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 14:00:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    SQL State pruning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements state pruning for the SqlMerkleState.  It adds two new operations, one to update a change log and the other to perform the pruning operation.

It removes the use of the index in get_leaves and goes directly against the tree node table using another recursive query - in order to support the appropriate branching needs in the state pruning tests (i.e. one parent root, two successor roots).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 02:24:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/174" class=".btn">#174</a>
            </td>
            <td>
                <b>
                    Order get path results by depth
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change enforces an order on the get_path results by the depth in the tree.  This guarantees that the nodes returned will be in depth-first order.

It fixes a serious issue where the trees produced were not correct.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 15:18:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    Remove unnecessary DB test URL loading
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes a duplicate URL loading from the environment variable for tests.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 15:15:08 +0000 UTC
    </div>
</div>

