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
                PR <a href="https://github.com/hyperledger/cactus/pull/1822" class=".btn">#1822</a>
            </td>
            <td>
                <b>
                    Johnhomantaring/issue1373
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1373
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 11:19:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1821" class=".btn">#1821</a>
            </td>
            <td>
                <b>
                    docs: changes to BUILD.md and CONTRIBUTING.md #1792
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes: #1792

Signed-off-by: ruzell22 <ruzell.vince.aquino@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 11:19:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1820" class=".btn">#1820</a>
            </td>
            <td>
                <b>
                    fix(security): address CVE-2021-23337
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1778
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 07:55:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1819" class=".btn">#1819</a>
            </td>
            <td>
                <b>
                    1776: Regular-Expression-Denial-of-Service-in-mime
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Affected versions of mime are vulnerable to regular expression denial of service when a mime lookup is performed on untrusted user input.

Action Applied:
Updated to version 3.

![mime](https://user-images.githubusercontent.com/55821921/151470107-a2f6678a-83a5-4745-bc98-e34b51718c58.png)
![mime3 0](https://user-images.githubusercontent.com/55821921/151470114-c7ba5cb6-c366-41e1-b006-87b4a8b8275a.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 01:18:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1818" class=".btn">#1818</a>
            </td>
            <td>
                <b>
                    refactor(cmd-socket-server, cartrade): use cmd-socket-server as a module 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Add module exports to cmd-socket-server, change it's usage in cartrade sample app.
- Cleanup redundant imports in cartrade.
- Add new method of starting `cmd-socket-server` with BLP (like cartrade) - `startCactusSocketIOServer` call.
- Old way of copying `BLP_config` is still supported, so other samples should work without a change.

Closes: #1817
Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

More details in the issue description.

Depends on #1813
- actually, it depends on one of the previous commits, but I don't want to introduce complex dependency graph and I "chain" them one after another :)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 15:15:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1816" class=".btn">#1816</a>
            </td>
            <td>
                <b>
                    fix(security): address CVE-2021-23358
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes: #1775 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 09:39:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1814" class=".btn">#1814</a>
            </td>
            <td>
                <b>
                    test: fix htlc eth besu initialize-endpoint-invalid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1684

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 12:07:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1813" class=".btn">#1813</a>
            </td>
            <td>
                <b>
                    refactor(indy-testnet) improve setup and tools of indy-testnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                This is a step before moving discounted-cartrade into container.

I've divided this PR into two commits for clarity. First one changes the logic and code, second is reorganization of different indy-testnet components (I've moved them around a little). If they were in single commit it'd be hard to follow the changes, I think :)

Documentation for components affected by this commit is outdated now, I'll update it after I finish my changes on them.

Depends on #1800

Depends on #1806

## refactor(indy-testnet) improve setup and tools of indy-testnet 
- `req_discounted_cartrade.py` - reuse proof when possible, add new flags to force new proof generation and to ignore discounted-cartrade request to simplify tests, put this tool into container.
- `testsock.js` - fix formatting, add missing package, use new validator address (nginx).
- Refactor all indy-testnet Dockerfiles according to docker best practices, reduce container size and complexity.
- Use nginx as a proxy to validator (as documented). 

## refactor(indy-testnet): organize indy-testnet components
- Move and adjust indy validator Dockerfile from `tools/docker/indy-testnet` to it's sources in `packages-python/cactus_validator_socketio_indy`.
- Rename indy validator dir from `cactus_validator_socketio` to `cactus_validator_socketio_indy`.
    - @izuru0 @petermetz What naming convention should be used for python packages? Is proposed name OK (it's based on current naming), or maybe we should use naming from `packages/`, i.e. `cactus-plugin-ledger-connector-indy-socketio`
- Rename `clientbase` image to `indy-sdk-cli`, move it to separate dir in `tools/docker`.
- Adjust paths in `indy-testnet` docker-compose, add dependency to start nginx after validator.
- Commit empty dir `tools/docker/indy-testnet/indy_pool/sandbox` directly to repo, remove redundant setup script.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 12:03:30 +0000 UTC
    </div>
</div>

