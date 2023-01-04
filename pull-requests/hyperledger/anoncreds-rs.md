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
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    build: Add build for ios and android
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Depends on #43 

closes #45 
closes #46 

- I had to patch openssl-src-rs, nothing functional, https://github.com/alexcrichton/openssl-src-rs/compare/release/111...blu3beri:openssl-src-rs:release/111 as it did not provide a build script for the target `aarch64-apple-ios-sim`. Since they do not accept non-security fixes for this branch we can not get this upstream, unless we depend upon openssl 3.

Work funded by the Government of Ontario.

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 13:42:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/43" class=".btn">#43</a>
            </td>
            <td>
                <b>
                    Added header files and generator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work funded by the Government of Ontario.

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 13:23:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/40" class=".btn">#40</a>
            </td>
            <td>
                <b>
                    Integrate indy-utils into anoncreds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #33 

Draft PR for removing / integrating the indy-utils within the anoncreds package

- NOTE: indy-vdr relies on the indy-utils package so there will some minor duplicate code.
  (e.g. base64/58)

Work funded by the Government of Ontario.

Signed-off-by: blu3beri <blu3beri@proton.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 14:05:03 +0000 UTC
    </div>
</div>

