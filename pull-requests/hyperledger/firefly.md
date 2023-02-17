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
                PR <a href="https://github.com/hyperledger/firefly/pull/1191" class=".btn">#1191</a>
            </td>
            <td>
                <b>
                    Update deprecated GitHub actions stuff
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/1187 and should address all of the warnings we currently have in our GitHub action runs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 21:11:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    Fix nightly integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously we were passing the `--blockchain-node` flag for all integration tests. The `ff init fabric` subcommand does not support this flag though, so it fails to create the test stack.

Here is an example of a failed run where this happened: https://github.com/hyperledger/firefly/actions/runs/4189374980/jobs/7261623960#step:6:139

```
ff -v --ansi never init fabric --prometheus-enabled --database sqlite3 firefly_e2e 2 --blockchain-node fabric --token-providers erc20_erc721 --manifest ../../manifest.json --sandbox-enabled=false --multiparty=true
Error: unknown flag: --blockchain-node
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 19:24:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1189" class=".btn">#1189</a>
            </td>
            <td>
                <b>
                    Add version to log output and fix Dockerfile to include it
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger/firefly/issues/1186
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 18:54:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    Fix typo in private & broadcast blob upload docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">documentation</span>
            </td>
            <td>
                I assume this should say `multi-part` (as in the MIME type) as opposed to `multi-party`

Signed-off-by: Matthew Whitehead <matthew1001@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 08:46:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1184" class=".btn">#1184</a>
            </td>
            <td>
                <b>
                    Fix path in Fabric test-network tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While re-running this tutorial I noticed that one of the paths to a key seemed incorrect. I have successfully run through it using the updated path in this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 16:09:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1183" class=".btn">#1183</a>
            </td>
            <td>
                <b>
                    remove near tutorial
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
        Created At 2023-02-13 15:21:57 +0000 UTC
    </div>
</div>

