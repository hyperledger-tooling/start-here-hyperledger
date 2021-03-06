---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    Rename tokens "https" plugin to "fftokens"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The name "https" is too generic - the plugin represents a way to map token operations
like pool, mint, and transfer into a specific HTTP+websocket protocol. Therefore a
specific, unique name is appropriate.

Also changed the config key from "connector" to "plugin" (since its purpose is to
affect which plugin FireFly loads from the map).

Added migration paths for both changes so that the CLI and any existing stacks can
have time to be updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 14:41:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    Add additional fields to TokenPool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                All token pools should record the connector that created them, may optionally
include a token symbol, and may (in the near future) be linked to a message.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 00:50:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    Swagger bug fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #199 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 20:43:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    Replace operation "info" with separate "input" and "output" fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Existing field has evolved to always contain plugin-specific data generated upon
completion of the operation. There is also a (separate) use case for storing
input data upon creating the operation, to support e.g. retryability.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-21 16:38:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Factor out "PersistTransaction" as a common database utility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                No idea where would be the appropriate place for this... but this general logic of validating and marking
a transaction complete is going to be needed outside of `events` (specifically, tokens look to be
introducing a new type of transaction that will be marked complete by a call in `syshandler`).

This logic is all transaction- and database-related (not particularly related to events). It's also not
particular to a specific database (ie SQL), although some of the checks could be pushed down into
the SQLCommon handler. Looking for input on whether a common utility like this is a good idea, or
if there's a better way to handle this common logic across packages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-20 16:05:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    Small fixes to token accounts
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
        Created At 2021-09-16 20:19:35 +0000 UTC
    </div>
</div>

