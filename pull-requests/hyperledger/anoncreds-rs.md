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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    chore: cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removed some of the unused delta related code
- Moved the revocation registry to its own file
- Some other minor fixes that do not change the functionality directly

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 07:35:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    build: remove duplicate name key
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
        Created At 2023-04-05 11:19:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    chore: update name in build-universal
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
        Created At 2023-04-05 11:18:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    chore: regenerated yarn lock file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - In response to: https://github.com/hyperledger/anoncreds-rs/security/dependabot/1

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 11:01:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    build(python): added CI/CD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Co-authored-by: blu3beri <blu3beri@proton.me>
Co-authored-by: Vickysomtee <victor@animo.id>

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 12:55:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    chore: update version to dev.14
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
        Created At 2023-04-04 11:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    fix(js): inconsistencies in create revocation state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes some inconsistencies and issues encountered when testing proving of revocable credentials. There's probably a few things that are broken in the verification / issuance as well, but I've mostly focused on the holder role now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-02 19:18:13 +0000 UTC
    </div>
</div>

