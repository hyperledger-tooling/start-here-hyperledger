---
layout: default
title: firefly-fir
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-fir
---

# firefly-fir <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-fir){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-fir/pull/18" class=".btn">#18</a>
            </td>
            <td>
                <b>
                    FIR-18: Blockchain confirmation listeners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                > Putting my proposal in a comment for now, and will work through discussion in the Github item before working to finalize the FIR document

Currently in FireFly you can:
- Listen for a reliable stream blockchain events emitted from successfully executed smart contract logic.
- Get a success/failure event from an `operation` that you submit via your particular FireFly server

However, there is a common pattern of programming that is not well served by this:
- Listen for all confirmed transactions (maybe matching some criteria)
- Query the events associated with that receipt
- Determine whether you want to process the events associated with that receipt

This requires a reliable ordered stream of receipts that are delivered in the order they are **confirmed** on the blockchain (the block containing them pass a point of finality), and the ability to decode the events associated with that receipt.

This issue proposes we:
- [ ] Design+add this new capability to the FFTM connector toolkit, as an optional feature a connector can implement
- [ ] Implement this feature in EVMConnnect
- [ ] Design+add a new `Blockchain confirmations` collection into FireFly core with appropriate listening/filtering
- [ ] Design+add a new semantic for decoding blockchain events on-demand into FireFly core
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 19:29:31 +0000 UTC
    </div>
</div>

