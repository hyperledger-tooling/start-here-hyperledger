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
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    feat: add zeroize as a feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - create zeroize feature (I am suprised that using `#[cfg(feature = "zeroize")]` worked without it being a feature. Maybe it picks up the dep)

Some not-so related changes included in this PR

- change blu3beri to berendsliedrecht GitHub name
- fix cargo issues and test work without default-features

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-09 09:28:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    fix(js): bump patched ref-napi/ffi-napi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the issue with types that appeared in https://github.com/hyperledger/aries-askar/pull/170#issuecomment-1708337866, here we update patched `ref-napi` and `ffi-napi` to embed their own types instead of using the ones from the original ones.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 20:43:02 +0000 UTC
    </div>
</div>

