---
layout: default
title: firefly-transaction-manager
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-transaction-manager
---

# firefly-transaction-manager <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-transaction-manager){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Pass options.signer for EthCompat mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                EVMConnect will separate out the option `options.signer: true` from the `options.methods: []` list of methods to match, so you can just request `signer`. Also so that even if no methods match we still set the signer.

This means a tweak to the EthCompat mode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 21:07:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Move completion log from "error" to "info"
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
        Created At 2022-08-29 17:49:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-transaction-manager/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Integrating sprig into gasOracle.Template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                http://masterminds.github.io/sprig/ is a common supplemental library for Go templating that has handy functions for ints and floats.

For oracle templates where we need to convert from gwei to wei, and /or convert from float to int, these utility functions can be very useful. This also provides us with a good starting point of examples in the event we ever need to write our own Go template functions such as converting from hex to bigints, etc.

Thanks @peterbroadhurst for doing the hard part of getting everything in place.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 04:15:35 +0000 UTC
    </div>
</div>

