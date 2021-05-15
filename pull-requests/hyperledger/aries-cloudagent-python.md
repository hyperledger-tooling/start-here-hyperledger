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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1169" class=".btn">#1169</a>
            </td>
            <td>
                <b>
                    Repair marshmallow duplicate schema warning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Address https://github.com/hyperledger/aries-cloudagent-python/issues/1166
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 19:36:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    Holder reject proof req on bad attr value restriction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Address https://github.com/hyperledger/aries-cloudagent-python/issues/1163 partially: have holder refuse to send hopeless proof request to indy-sdk.

Ultimately the handlers should send problem reports - that's a bigger job and needs its own PR
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-12 14:55:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1164" class=".btn">#1164</a>
            </td>
            <td>
                <b>
                    Local jsonld for unit tests
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
        Created At 2021-05-11 16:23:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1162" class=".btn">#1162</a>
            </td>
            <td>
                <b>
                    retain unrecognizable decorators as opaque data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                RFC 11 suggests a looser interpretation than our original.
Address https://github.com/hyperledger/aries-cloudagent-python/issues/1147

Signed-off-by: sklump <srklump@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 15:56:29 +0000 UTC
    </div>
</div>

