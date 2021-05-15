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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Update workload to handle TooManyRequests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates workload to handle the TooManyRequests response from a target by sleeping and attempting to submit the same batch until successful.

Running the `transact workload` command with -vv will print a message in the logs stating that the batch is being resubmitted when a `TooManyRequests`  message is received from the target 

### **Testing:**

1. Start two splinter nodes with the experimental feature "back-pressure" 
2. Create a circuit between the nodes, ensure that the scabbard version is set to 2 when creating the circuit
3. Use scabbard CLI to upload the smallbank smart contract contract
4. Use the transact CLI to start a workload, for example:
```
transact workload --targets http://splinterd-beta:8085/scabbard/<circuit-id>/<service-id> \
--key <private-key-path> \
--target-rate 5 \
--update 2 \
--workload smallbank \
-vv
```
The log messages should look something like this
```
Smallbank-Workload-0: May-11-2021 21:42:38.758, Sent: 10, Queue Full 0, Batches/s 4.914
Smallbank-Workload-0: May-11-2021 21:42:40.838, Sent: 9, Queue Full 0, Batches/s 4.326
Smallbank-Workload-0: May-11-2021 21:42:43.123, Sent: 10, Queue Full 0, Batches/s 4.377
Smallbank-Workload-0: May-11-2021 21:42:45.168, Sent: 9, Queue Full 0, Batches/s 4.402
Received TooManyRequests message from target, attempting to resubmit batch
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-11 18:59:25 +0000 UTC
    </div>
</div>

