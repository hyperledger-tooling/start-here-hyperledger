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
                PR <a href="https://github.com/hyperledger/firefly/pull/1022" class=".btn">#1022</a>
            </td>
            <td>
                <b>
                    [identity-tutorial] identity tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tutorial to guide user through creating a Custom Identity in FireFly.

References https://github.com/hyperledger/firefly/issues/621
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 19:10:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1021" class=".btn">#1021</a>
            </td>
            <td>
                <b>
                    Allow any plugin to terminate the system on a bad event
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Terminating the system is better than leaving it up in a crippled state.

Closes #957
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 18:52:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1019" class=".btn">#1019</a>
            </td>
            <td>
                <b>
                    Clean up event manager unit tests
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
        Created At 2022-08-30 17:25:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1018" class=".btn">#1018</a>
            </td>
            <td>
                <b>
                    add another account for fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Anna Jackson <anna.jackson@kaleido.io>

Fixes #1011 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 09:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1017" class=".btn">#1017</a>
            </td>
            <td>
                <b>
                    adds `fetchreference` to /events/:id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When provided, firefly will include the record that the `ref` field references in the response body.

closes #1016 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 02:33:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1015" class=".btn">#1015</a>
            </td>
            <td>
                <b>
                    Add firefly-signer to manifest
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
        Created At 2022-08-29 19:21:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1012" class=".btn">#1012</a>
            </td>
            <td>
                <b>
                    Namespaces reference section + moonbeam docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                docs are live here: https://shorsher.github.io/firefly/head/reference/namespaces.html


in a chain with #966 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 15:33:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1010" class=".btn">#1010</a>
            </td>
            <td>
                <b>
                    Update Good First Issue Link
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
        Created At 2022-08-29 14:18:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1009" class=".btn">#1009</a>
            </td>
            <td>
                <b>
                    Ensure new namespaces are up during multi_tenancy test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1008
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-26 16:39:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1006" class=".btn">#1006</a>
            </td>
            <td>
                <b>
                    Verify integrity of group for private messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This extends the verification of off-chain node identities to not only verify that the sender's DX node is properly related to the message author identity, but _also_ that the private message group contains a member corresponding to that combination of node+identity.

For pinned messages, this verification is now all deferred to the aggregator. For unpinned, this verification continues to be inline on the DX callback.

Open questions not addressed in this PR:
- should we be caching group lookups?
- should we validate that the _batch_ group and author match the _message_ group and author?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 14:02:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1005" class=".btn">#1005</a>
            </td>
            <td>
                <b>
                    Create a centralised cache manager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Create a centralised cache manager as described in #943 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 09:43:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1004" class=".btn">#1004</a>
            </td>
            <td>
                <b>
                    Ensuring Empty List is Provided for FFDX Init on Zero Peer Nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                DX's being implemented in languages like Typescript do not treat `null` as a valid, empty JSON array which was causing problems. Core would get a `500` from DX:
```
{"@timestamp":"2022-08-24T17:49:59.714Z","breq":"8CWznOwK","dx":"https","level":"debug","message":"==\u003e POST http://firefly-dx.infra.svc:3000/api/v1/init","pid":"1"}
{"@timestamp":"2022-08-24T17:49:59.720Z","breq":"8CWznOwK","dx":"https","level":"error","message":"\u003c== POST http://firefly-dx.infra.svc:3000/api/v1/init [500] (5.67ms)","pid":"1"}
```
and we'd see DX error with:
```
2022-08-24T17:49:52.646Z [ERROR]: Unexpected token n in JSON at position 0 lib/request-error.ts
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 20:18:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1003" class=".btn">#1003</a>
            </td>
            <td>
                <b>
                    Upgrade firefly-common to v1.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Includes required syntax changes to go with https://github.com/hyperledger/firefly-common/pull/33
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 18:58:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1002" class=".btn">#1002</a>
            </td>
            <td>
                <b>
                    Add tool for auditing blockchain event order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an alternative to #998, written in Go rather than bash.

Not sure where we should put scripts if we keep adding them... do we just keep adding root level folders like this?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 15:35:36 +0000 UTC
    </div>
</div>

