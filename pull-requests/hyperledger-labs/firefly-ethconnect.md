---
layout: default
title: firefly-ethconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/147" class=".btn">#147</a>
            </td>
            <td>
                <b>
                    Allow including method inputs with subscribed events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Passing {"inputs": true} when initializing an event stream will cause each
event to include two new fields - inputMethod will be the name of the method
that emitted the event, and inputArgs will be a map of the args passed in
when the method was called.

This can be reviewed in parallel with #141, although they share one commit
containing some generic helpers for decoding transaction info.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 16:17:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/146" class=".btn">#146</a>
            </td>
            <td>
                <b>
                    Move contract sorting up to contractStore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Makes the contractStore unit tests pass more reliably.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 17:39:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/145" class=".btn">#145</a>
            </td>
            <td>
                <b>
                    Rename methods on ContractStore for consistency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Follow-up to https://github.com/hyperledger-labs/firefly-ethconnect/pull/144 - makes the API of the new ContractStore type just a bit clearer and friendlier.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 15:44:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-ethconnect/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    Split "contracts" package into "contractgateway" and "contractregistry"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The new "contractregistry" package has minimal dependencies and can be used from anywhere
to lookup contracts/ABIs, while the "contractgateway" package remains large and pulls in nearly
everything.

This will facilitate future enhancements where we want to do ABI lookups from outside the gateway
(such as from the "events" package).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 19:29:27 +0000 UTC
    </div>
</div>

