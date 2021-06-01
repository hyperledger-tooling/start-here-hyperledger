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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    TooManyRequests response bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a bug in the recent update to handle `TooManyRequests`. Previously if control-c was pressed while the `slow_rate` method was attempting to resubmit a batch the workload would not stop until `slow_rate` had returned and it would usually result in a panic caused by a divide by zero error.

The following changes are added in this PR to fix this bug:
- After each time `slow_rate` is called the time and total batches counters used to calculate the effective submission rate are reset
- The `slow_rate` method is updated to default to 1 second of sleep if the effective rate is calculated to be 0, this avoids any possible divide by zero errors that were possible before
- A `receiver` argument is added to the `slow_rate` method, the method uses the receiver to check if a shutdown message has been sent each time it loops
- The `slow_rate` method is updated to return a boolean representing whether or not a shutdown message was sent. If `slow_rate` returns `true` the loop will break and the workload will stop

### **Testing:**
1. Start two splinter nodes with the experimental feature "back-pressure"
2. Create a circuit between the nodes, ensure that the scabbard version is set to 2 when creating the circuit
3. Use scabbard CLI to upload the smallbank smart contract
4. Use the transact CLI to start a smallbank workload, for example:
```
transact workload --targets http://localhost:8085/scabbard/<circuit-id>/<service-id> \
--key <private-key-path> \
--target-rate 5 \
--update 2 \
--workload smallbank \
-vv
```
5. Control-c immediately after seeing the log message:
```Received TooManyRequests message from target, attempting to resubmit batch```
check that the log shows:
```
Shutting down worker Smallbank-Workload-0
Worker received shutdown
```
and the workload stops
6. Run the workload command again
7. Control-c while batches are being successfully submitted
check that the same shutdown log message shows:
```
Shutting down worker Smallbank-Workload-0
Worker received shutdown
```
and the workload stops
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 21:58:56 +0000 UTC
    </div>
</div>

