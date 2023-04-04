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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    fix(rn): link secret is string instead of object
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Link secret has changed from object to just a string, but this wasn't reflected in the C++ layer
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-02 14:53:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    fix: correctly generate header
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
        Created At 2023-04-01 12:45:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/174" class=".btn">#174</a>
            </td>
            <td>
                <b>
                    chore: increase version to dev.13
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
        Created At 2023-04-01 10:17:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/173" class=".btn">#173</a>
            </td>
            <td>
                <b>
                    fix: cred def should still use master_secret
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As discussed in https://github.com/hyperledger/aries-framework-javascript/pull/1415
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 10:13:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/172" class=".btn">#172</a>
            </td>
            <td>
                <b>
                    feat(js): revocation status list from json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This add support to create a revocation status list from json in the JS wrapper. The method was already availalbe in the ffi layer as `anoncreds_revocation_list_from_json`, but I changed it to `anoncreds_revocation_status_list_from_json` as that aligns more with the rest of the naming. If we choose to call it `revocation_list` we should change it everywhere at once.

Also fixes a few small issues in the RN wrapper.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-01 10:02:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/170" class=".btn">#170</a>
            </td>
            <td>
                <b>
                    build: remove macos from check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Renamed `check` to `test` to reflect the cargo subcommand
- Removed `macos` from `test` to avoid unnecessary macos runs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-31 08:42:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    chore(ci): Update to upload-artifact v3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should resolve the deprecation warnings in actions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 22:41:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    chore: update version to dev.12
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
        Created At 2023-03-30 14:10:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/167" class=".btn">#167</a>
            </td>
            <td>
                <b>
                    feat: schema ordering
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fix: use c_char for lower rust version
  - closes #163
- fix: ordering of schemas is as input
  - closes #136 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 09:37:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    chore(python): added pyproject.toml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #154 

@dbluhm any chance you can review this? I followed some guides, and the demo is working, but python setup still remains a small mystery to me :).

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 09:01:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    Try BuildJet
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
        Created At 2023-03-29 15:43:49 +0000 UTC
    </div>
</div>

