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
                PR <a href="https://github.com/hyperledger/transact/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    Add default key location
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update the `create_cylinder_jwt_auth_signer_key` function to check the default location, ~/.cylinder/keys, if no `--key` argument is given.
- Update the following CLI commands to not require the `--key` arg: `command set-state`, `command get-state`, `command show-state`, `playlist submit` and `workload`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 17:34:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    Fix clippy errors
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
        Created At 2021-12-02 16:11:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    Move `CommandTransactionBuilder`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a copy of the `CommandTransactionBuilder`, from the `family::command::workload` module, to a new `family::command::transaction_builder` module behind a new feature "family-command-transaction-builder" and re-export it from `family::command`. Additionally, depreciate the copy of the builder in the workload module.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 16:12:30 +0000 UTC
    </div>
</div>

