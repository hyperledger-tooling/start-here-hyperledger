---
layout: default
title: firefly-dataexchange-https
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-dataexchange-https
---

# firefly-dataexchange-https <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-dataexchange-https){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    Fix peeradd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I found that `addSecureContext` was not reliably causing a working TLS context on startup of the firefly CLI with the e2e test.
It looks like simplifying to `setSecureContext ` instead (without supplying a particular hostname) is the right thing to do.

Note in PR chain with #25
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 17:47:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    Incomplete uploads
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains:
- A fix to the Transform that does hashing on upload, to avoid incomplete data transfers
- Fix the `sender` for blobs arriving from other members
- Fixes to make Typescript happy (implicit any errors preventing my build running)
- Additional logging to diagnose cases where events are not flowing, including an event ID
- Simplified logger that works with the docker compose output in firefly-cli

With e2e testing, I was finding:
- The binary data stored in the blob store was incomplete
- The hash was incorrect (this was detected on the FireFly core side)

After much debugging to see if core was somehow not propagating the data stream through correctly, I tried running the DX locally, and I found I was getting the following error:
```
{"name":"app.ts","hostname":"peters-mbp-3.lan","pid":65130,"level":30,"msg":"New WebSocket delegate assigned","time":"2021-06-20T03:00:22.784Z","v":0}
(node:65130) UnhandledPromiseRejectionWarning: Error [ERR_CRYPTO_HASH_FINALIZED]: Digest already called
    at Hash.update (internal/crypto/hash.js:79:11)
    at Transform.<anonymous> (/Users/peterbroadhurst/dev/photic/firefly-dataexchange-https/src/handlers/blobs.ts:50:12)
    at Generator.next (<anonymous>)
    at /Users/peterbroadhurst/dev/photic/firefly-dataexchange-https/src/handlers/blobs.ts:42:71
    at new Promise (<anonymous>)
    at __awaiter (/Users/peterbroadhurst/dev/photic/firefly-dataexchange-https/src/handlers/blobs.ts:38:12)
    at Transform.transform [as _transform] (/Users/peterbroadhurst/dev/photic/firefly-dataexchange-https/src/handlers/blobs.ts:79:20)
    at Transform._read (_stream_transform.js:205:10)
    at Transform.Readable.read (_stream_readable.js:481:10)
    at flow (_stream_readable.js:992:34)
(Use `node --trace-warnings ...` to show where the warning was created)
(node:65130) UnhandledPromiseRejectionWarning: Unhandled promise rejection. This error originated either by throwing inside of an async function without a catch block, or by rejecting a promise which was not handled with .catch(). To terminate the node process on unhandled promise rejection, use the CLI flag `--unhandled-rejections=strict` (see https://nodejs.org/api/cli.html#cli_unhandled_rejections_mode). (rejection id: 1)
(node:65130) [DEP0018] DeprecationWarning: Unhandled promise rejections are deprecated. In the future, promise rejections that are not handled will terminate the Node.js process with a non-zero exit code.
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 17:35:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-dataexchange-https/pull/23" class=".btn">#23</a>
            </td>
            <td>
                <b>
                    Add metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Gabriel Indik <gabriel.indik@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 20:13:56 +0000 UTC
    </div>
</div>

