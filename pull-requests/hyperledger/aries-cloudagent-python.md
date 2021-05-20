---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    Issue cred store cred done
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-19 19:54:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1183" class=".btn">#1183</a>
            </td>
            <td>
                <b>
                    Align with rfcs for error states in issue cred and present proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RFCs 36, 37, 453 state that exchange states go to null on both sides on error; 454 uses "abandoned".

This work sets states accordingly where possible (unless there is no such record or the problem is storage itself), but does not (yet) send problem reports - that's another PR for the near-ish future.

In issue-credential, separate store-credential from send-ack: whether storage succeeds or fails, the protocol owes an ack because acknowledgement is to credential receipt, not storage.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 13:52:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    DIDX create-request [return ConnRecord]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work left from #1174 and #1137.

- /didexchange/create-request now return ConnRecord
- Based upon feedback from @domwoe and  @andrewwhitehead, this will make it more consistent
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 00:24:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1180" class=".btn">#1180</a>
            </td>
            <td>
                <b>
                    fix: use injected document loader for pyld calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 08:34:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1179" class=".btn">#1179</a>
            </td>
            <td>
                <b>
                    Add `resolve_with_metadata` method to DID resolver
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This metadata includes information on how the DID was resolved, enabling the caller to make decisions about whether it accepts DID Documents resolved remotely or from a particular resolver, etc.

Props to @Luis-GA for doing most of the legwork on this feature.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-15 17:37:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1178" class=".btn">#1178</a>
            </td>
            <td>
                <b>
                    fix: don't load indy resolver if no indy ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 15:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1176" class=".btn">#1176</a>
            </td>
            <td>
                <b>
                    Make BaseResolver.supports async and prefer regex matching
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR extends the `BaseResolver.supports` method to be asynchronous and to take a `Profile` to support such use cases as retrieving resolver connections from storage and checking DIDs supported by those resolver connections. Additionally, this PR adds `supported_did_regex` as a value intended to be implemented by subclasses of `BaseResolver` and used in the default `supports` implementation. This changes the previous behavior of matching on the DID method alone to regex matching, granting more flexibility in how resolvers are selected to handle DID resolution.

`supported_methods` remains functional to prevent breaking resolver plugins already in the wild but is marked as deprecated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 03:48:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1175" class=".btn">#1175</a>
            </td>
            <td>
                <b>
                    unit tests cover new core/dispatcher code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 18:21:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1174" class=".btn">#1174</a>
            </td>
            <td>
                <b>
                    DID Exchange - Create and send requests against implicit invitations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1137 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 16:51:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1171" class=".btn">#1171</a>
            </td>
            <td>
                <b>
                    propagate comment in auto for issue-cred v1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/aries-cloudagent-python/issues/1167
Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-13 11:13:22 +0000 UTC
    </div>
</div>

