---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2190" class=".btn">#2190</a>
            </td>
            <td>
                <b>
                    test(verifier-client): add stress test and fix a memory leak
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add a new package `@hyperledger/cactus-test-verifier-client` for verifier-client stress and
  functional tests that involve multiple packages.
- Add stress test for verifier-client that reports memory usage of repeated operation
  on `cactus-plugin-ledger-connector-go-ethereum-socketio` connector plugin.
- Fix a memory leak in `SocketIOApiClient` - free socket listeners when they are no longer needed.
- Fix `cactus-plugin-ledger-connector-go-ethereum-socketio` - use single a web3 connection
  (with keep-alive/reconnect) instead of spawning new one for each request.
  Previous solution was causing connection issues in stress testing.

Depends on: https://github.com/hyperledger/cactus/pull/2089
Closes: https://github.com/hyperledger/cactus/issues/2189

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

-------------

Please review only the last commit, the others are dependencies.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-07 16:34:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2188" class=".btn">#2188</a>
            </td>
            <td>
                <b>
                    ci(github): upgrade actions/checkout to v3.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Project-wide search and replace for all occurrences of the
checkout GH workflow action so that it is at the current
latest stable release version which is v3.1.0

Fixes #2187

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-04 00:15:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2186" class=".btn">#2186</a>
            </td>
            <td>
                <b>
                    chore(release): publish v1.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is needed because of the botched (congrats Peter) v1.1.0 release which we attempted to fix by adding a new workflow action that gets triggered on tags and then re-applying (delete+re-tag) the v1.1.0 release tag.
Only after all this was it discovered that the workflow action meant to push the 1.1.0 npm artifacts will not get triggered on the v1.1.0 tag because the workflow file got added in a commit prior to v1.1.0 so the only way to fix it would be to:
1. have direct push access ot npm once again (temporarily) until we can issue the 1.1.0 release or
2. re-write the git history of the upstream main branch (a big no-no unless we absolutely must do that for whatever reason)

TLDR: Issuing a v1.1.1 release here basically just to test whether the auto-publishing of packages with the new workflow works at all or not. If it has bugs or does not work for whatever other reason we will need to itreate on the workflow file and then issue a v1.1.2 and more of those as needed until we figure out the auto-publishing so that it "just works" 

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-02 21:25:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2185" class=".btn">#2185</a>
            </td>
            <td>
                <b>
                    feat(cbdc-bridging-app): implementation of CBDC bridging example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR presents a new example to demonstrate the capabilities of Cactus. This application demonstrates a CBDC bridging between a Fabric and a Besu network using the ODAP business logic plugin, a protocol under standardization for cross-chain operations in the IETF.

The goal is to demonstrate the use of npm packages of Cactus so that anyone can build a solution such as this. (Some dependencies are not using npm packages and the Dockerfile is not functional yet since some npm packages are not available yet – an example is the ODAP plugin).

Summary of the contributions:
* CBDC application backend (setting up and interacting with the underlying ledgers through smart contracts)
* CBDC application frontend (UI demonstrating the use of the app)
* Add support for multiple organizations in some operations in the FabricTestLedger
* Add support for minting some Ether to a given address in the BesuTestLedger

More documentation will be added in the next weeks.

Signed-off-by: André Augusto <andre.augusto@tecnico.ulisboa.pt>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-02 10:43:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/2184" class=".btn">#2184</a>
            </td>
            <td>
                <b>
                    fix(tools): ghcr-quorum-multi-party-all-in-one pip install
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgraded the base image version from
`docker:20.10.3-dind`
to
`docker:20.10.21-dind`
which ships with newer rust versions through apk
by default and thereby fixing the issue of the rust
compiler version being not new enough for
docker-compose.

Fixes #2183

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-02 05:26:34 +0000 UTC
    </div>
</div>

