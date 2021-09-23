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
                PR <a href="https://github.com/hyperledger/transact/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Restrict just doc to published configuration 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change restricts the `just doc` task to only apply the rustdoc configuration that would be run for the published crates.  Prior to this commit, `just doc` would run the whole workspace, which causes file name conflicts between libtransact and transact-cli.

Also fixes some resulting warnings from this change.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 22:27:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    SqlMerkleState typo fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 19:01:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Remove outdated comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes an outdated comment, left over from the development process.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 17:51:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Correct feature guard for diesel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change corrects the feature guard for diesel to "diesel", making it less dependent on the feature defined in libtransact's Cargo.toml, and merely dependent on whether or not the optional dependency is included in the set of active features.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 15:42:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/190" class=".btn">#190</a>
            </td>
            <td>
                <b>
                    SqlMerkleState integration test re-org
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR moves some use statements, statics and functions around, for consistent file organization.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 14:28:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/189" class=".btn">#189</a>
            </td>
            <td>
                <b>
                    Move sqlite and postgres specifics into own files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change moves the sqlite- and postgres-specific implementations of state-related traits (and internal traits for SqlMerkleState implementation) into their own respective sub-modules.  This brings the root state::merkle::sql module in line with the rest of the sql sub-modules.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 21:45:41 +0000 UTC
    </div>
</div>

