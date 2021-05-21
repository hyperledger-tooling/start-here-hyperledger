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
                PR <a href="https://github.com/hyperledger/transact/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    Run just recipes in CI
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
        Created At 2021-05-20 01:05:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    Move Database-backed MerkleTree to kv submodule
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change moves the existing merkle tree implementation to a kv submodule and re-exports it from the original module. This provides a space for additional back-end implementations.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 21:49:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    Fix Transact docker builds with Docker Compose 1.28+
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
        Created At 2021-05-18 19:11:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    Change wait time between batch submit responsively
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Transact waits the full time between the end of one batch submit and the
next regardless of how long the submit takes. This can make the target
submission rate and the actual submission rate be very different.
This change alters the time between submissions based on how long the
current submission took and a "best guess" for how long they usually
take.
Ideally this will more tightly tie the target and actual submission rate.

Signed-off-by: Caleb Hill <hill@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 13:02:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/135" class=".btn">#135</a>
            </td>
            <td>
                <b>
                    Add InvalidStateError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds the InvalidStateError basic error, copied from the splinter library ( Cargill/splinter@f0cb463b8d7b7ba1dc1000ba78c8ef4c8d32e183)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 19:14:08 +0000 UTC
    </div>
</div>

