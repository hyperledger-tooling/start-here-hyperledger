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
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    chore(ci): switch to dedicated Anoncreds runners
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
        Created At 2023-04-19 00:15:40 +0000 UTC
    </div>
</div>

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

