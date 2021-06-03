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
                PR <a href="https://github.com/hyperledger/transact/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    Add patch notes for 0.3.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ryan Banks <rbanks@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 16:16:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/152" class=".btn">#152</a>
            </td>
            <td>
                <b>
                    Generic Merkle State Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change updates the merkle state tests to use the state traits in all tests that don't involve pruning checks.  This will enable validating the SQL-backed implementation against the same tests.

Additionally, 

- Fixes a bug with error output of the trait implementations in the key-value implementation
- replaces panics with resume_unwind in the test wrappers
- Adds a `key()` accessor to `StateChange`, for convenience
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-02 14:35:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/151" class=".btn">#151</a>
            </td>
            <td>
                <b>
                    Backport - Update semver dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update sever from 0.9 to 1.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-01 15:20:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/149" class=".btn">#149</a>
            </td>
            <td>
                <b>
                    Add SQL operations for new SQL-backed merkle radix implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a set of operations that will support the SQL-backed merkle radix state implementation.  

A future PR will implement the radix tree over a sqlite db using these operations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 21:45:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/148" class=".btn">#148</a>
            </td>
            <td>
                <b>
                    Remove the clean dependency from just lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To get the old behavior, run "just clean; just build". This change makes
the clean optional, which is a more desirable developer workflow.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 20:08:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/147" class=".btn">#147</a>
            </td>
            <td>
                <b>
                    Update the semver dependency from 0.11 to 1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This version was recently released and this change was motivated solely to
track the most recent version.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-28 20:05:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/146" class=".btn">#146</a>
            </td>
            <td>
                <b>
                    Add MerkleRadixLeafReader trait
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This trait provides a generic leaf listing api, that matches the key-value backed implementation's provided method.

Additionally, implements this trait on the existing `kv::MerkleState`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 19:41:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/145" class=".btn">#145</a>
            </td>
            <td>
                <b>
                    Add examples/sabre_command to justfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is required to catch build, lint, and testing errors in this
example crate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 17:03:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    Remove env output from 'just build'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is undesirable output when running the command in the developer workflow.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 16:59:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/143" class=".btn">#143</a>
            </td>
            <td>
                <b>
                    Update Sha2::Sha512 usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update to work with the current version of sha2 used in transact.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 16:58:08 +0000 UTC
    </div>
</div>

