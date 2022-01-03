---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    Add regex for company name in header
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 17:44:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/373" class=".btn">#373</a>
            </td>
            <td>
                <b>
                    Add Performance Testing Details to README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding performance testing details to README
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 16:14:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/372" class=".btn">#372</a>
            </td>
            <td>
                <b>
                    [helm] Tokens ERC1155 Deployment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                TODOs
- [ ] https://github.com/hyperledger/firefly-tokens-erc1155/pull/50 merged
- [ ] https://github.com/hyperledger/firefly/pull/359 merged
- [ ] docs
- [ ] testing
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 14:15:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    Fixing Websocket Connections when Prometheus Metrics Enabled
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Uses my fork https://gitlab.com/hfuss/mux-prometheus (opened a PR against the original: https://gitlab.com/msvechla/mux-prometheus/-/merge_requests/11) so that the necessary `Hijack` method is implemented in the wrapper around `ResponseWriter` in order to fix #370 
* Enables Prometheus metrics when running E2E tests so that any bugs its middleware is introducing are noticed
* Adds the `ff_` prefix to the middleware metrics
* Ran `go mod tidy`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 21:40:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    Update dependencies for next release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Full round of dependency updates:
- Manifest updates to latest release of FabConnect 
- Go dependency update to latest across the board
- Truffle dependency update
  - Removed no longer required asset trail contract
  - Removed unused dependency on OpenZeppelin
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-29 17:05:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    Fix misspelled filename (bytetypes.go)
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
        Created At 2021-12-29 16:47:56 +0000 UTC
    </div>
</div>

