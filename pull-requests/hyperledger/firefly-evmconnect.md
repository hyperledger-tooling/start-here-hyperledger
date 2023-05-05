---
layout: default
title: firefly-evmconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-evmconnect
---

# firefly-evmconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-evmconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/82" class=".btn">#82</a>
            </td>
            <td>
                <b>
                    Update to fftm v1.2.11
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
        Created At 2023-05-03 20:35:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Error receipt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add `errorMessage` field to the receipt when a transaction fails by calling `debug_traceTransaction`.  Given that this is not certain to be implemented on all clients, we tolerate any errors and just omit the errorMessage from the receipt .

This has been tested on besu and quorum with a `require` statement in the contract causing the revert.  As yet I have been unable to prove that this is also effective in the case where there is not enough gas.  So not claiming that this fixes https://github.com/hyperledger/firefly-evmconnect/issues/60 just yet but it is a useful fix nonetheless.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-29 14:59:39 +0000 UTC
    </div>
</div>

