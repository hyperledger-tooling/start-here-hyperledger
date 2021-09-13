---
layout: default
title: firefly-fabconnect
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-fabconnect
---

# firefly-fabconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-fabconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Unit tests for eventstream
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added unit tests coverage for eventstream
- eliminate dependencies for `github.com/hyperledger/fabric` which doesn't follow go module versioning rules
- added `Unregister()` method to the `fabric/RPCClient` interface to allow better test-ability
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 12:10:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-fabconnect/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Enrich GET identity endpoint responses with certs and mspID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The certificates for the user and the CA as well as the MSP ID are necessary for building the full Fabric Identity from a simple user name, which follows the pattern `x509::{DN of user cert}::{DN of CA cert}`.

These are added to the `GET /identities/:id` calls only, not to the list calls (`GET /identities`) to avoid lengthy response time
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 14:12:05 +0000 UTC
    </div>
</div>

