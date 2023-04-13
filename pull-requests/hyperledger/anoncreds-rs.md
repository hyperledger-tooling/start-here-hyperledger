---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    fix(js): nonRevokedIntervalOverrides naming
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A very subtle option naming was preventing the non revoked interval overrides to get processed by Rust code: base Anoncreds interface was using `nonRevokedIntervalOverride` while NodeJS and ReactNative implementations are referring to it as `nonRevokedIntervalOverrides` (which makes more sense as it is an array of overrides).

Solves #191 and updates a bit API test to reflect the usage of this parameter.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 16:26:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    chore(ci): move to large GitHub runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 15:06:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/190" class=".btn">#190</a>
            </td>
            <td>
                <b>
                    fix: remove references to deltas in wrappers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In #185, `anoncreds_revocation_registry_delta_from_json` was removed, which caused the CI to fail for JS wrappers (that were still calling this function).

So here we are removing all references to RevocationRegistryDelta from both JS and Python wrappers. The latter did also have a reference to `anoncreds_revoke_credential` that is also missing in current code base.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 12:37:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/189" class=".btn">#189</a>
            </td>
            <td>
                <b>
                    fix(build): use cross for lower glibc compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 07:48:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/188" class=".btn">#188</a>
            </td>
            <td>
                <b>
                    fix(js): integer list struct types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Another issue found during testing credential revocation in AFJ: remove pointer for integer arrays
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 21:59:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    fix(js): revocation status list typo and optional timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some things I found while digging a bit with revocation status lists in JavaScript.

Also, maybe more for a discussion or separate issue, but I find a bit odd to have both `updateTimestamp()` and `update()` methods in `RevocationStatusList` class from JS API. It could be more straightforward to just have `update()` and, if the only defined parameter is the timestamp, it can call `anoncreds.updateRevocationStatusListTimestampOnly`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 18:23:40 +0000 UTC
    </div>
</div>

