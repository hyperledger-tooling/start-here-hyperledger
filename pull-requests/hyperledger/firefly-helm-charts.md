---
layout: default
title: firefly-helm-charts
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-helm-charts
---

# firefly-helm-charts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-helm-charts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-helm-charts/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    [0.6.0] Support for EVMConnect and FireFly v1.1.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes a new `firefly-evmconnect` chart so that multiple installations of EVMConnect can be made for different Ethereum-based chains (public or private).

The core `firefly` chart is then updated to include creating a single installation of `evmconnect`, and migrate the presumably existing `default` multi-party namespace to the new v1.1.x namespace config format (see the relevant [FIR](https://github.com/hyperledger/firefly-fir/pull/12) and [migration guide](https://github.com/hyperledger/firefly/wiki/Migration-Guide-for-v1.1.0)) while allowing for new, additional namespaces to be defined with however many additional plugins may be needed (via `config.extraDatabases`, `config.extraBlockchains`, etc.). Similarly, if users created other multi-party namespaces in their v1.0.x installations of FireFly, they will be able to define and migrate them using `config.extraNamespaces`.

`ethconnect` support within the chart is then deprecated in favor of `evmconnect`. And lastly, the ability to connect to _both_ `evmconnect` and a remote Fabconnect is supported with the choice of which to use for the `default` namespace. This allows users to create a multi-party namespace based on Fabric, but then have a gateway or additional multi-party namespace pointed to an Ethereum chain for example.

TODOs
- [x] `ci/` files for EVMConnect
- [x] Further test
- [ ] Finish docs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-30 01:51:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-helm-charts/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Fix a typo in several annotations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Chris Bygrave <chris.bygrave@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 08:30:11 +0000 UTC
    </div>
</div>

