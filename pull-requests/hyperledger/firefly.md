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
                PR <a href="https://github.com/hyperledger/firefly/pull/379" class=".btn">#379</a>
            </td>
            <td>
                <b>
                    Allow any company name in license header
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
        Created At 2022-01-03 20:44:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/378" class=".btn">#378</a>
            </td>
            <td>
                <b>
                    Fetch full history on all GitHub Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a followup to https://github.com/hyperledger/firefly/pull/377 which changes the setting in all the GitHub actions for this repo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 20:04:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    Set fetch-depth to get the full history in GitHub Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is to fix the linter failing while checking the header copyright date for files that were not changed this year. This change pulls the full git history in the checkout stage, similar to what would happen if a user did a `git clone` on their local machine.

This PR will likely need to be merged without a passing build, due to the fact that all builds are stuck needing this change.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 19:51:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/375" class=".btn">#375</a>
            </td>
            <td>
                <b>
                    Have DB creation script account for username
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This script previously made incorrect assumptions about the name of the database user and the name of the database. Providing connection strings with no db name initiates a connection using the username as the database name. Instead, the connection should always be made to the default `postgres` database.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-03 19:19:44 +0000 UTC
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
- [x] https://github.com/hyperledger/firefly/pull/359 merged
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

