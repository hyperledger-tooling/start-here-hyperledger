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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    Remove InternalError::reduce_to_string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This method is a wrapper around to_string that also logs a message if there is a source.  The logging and to_string call should be left to the caller.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 16:01:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    Add InternalError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds the InternalError basic error, copied from the splinter, as of commit Cargill/splinter@f0cb463b8d7b7ba1dc1000ba78c8ef4c8d32e183
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 17:25:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/132" class=".btn">#132</a>
            </td>
            <td>
                <b>
                    Allow transaction rates less than 1/sec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sometimes a rate of one a second is too high for a specific workload and
it is currently the slowest rate supported. This commit lets you set a
rate of less than 1 batch per second.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 15:53:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    Rename transact-command.md to transact-command.1.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the expected naming scheme.

Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 13:22:17 +0000 UTC
    </div>
</div>

