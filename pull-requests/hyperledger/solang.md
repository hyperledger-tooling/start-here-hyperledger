---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1086" class=".btn">#1086</a>
            </td>
            <td>
                <b>
                    remove seal prefixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Cyrill Leutwiler <bigcyrill@hotmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 09:46:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1085" class=".btn">#1085</a>
            </td>
            <td>
                <b>
                    Improve CI and other fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Solang CI already has python3, no need to install
- Docs needs git
- solang.io domain no longer registered (expired)
- Do not use ^ for crates
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-28 09:14:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1082" class=".btn">#1082</a>
            </td>
            <td>
                <b>
                    Make solang build with inkwell 0.1.0-beta.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Offender in Cargo.toml is:

`inkwell = { version = "^0.1.0-beta.4", features = ["target-webassembly", "target-bpf", "no-libffi-linking", "llvm13-0"], optional = true }`

I can't find any release notes for `inkwell`? I guess since everything green on our CI it is fine for us to ape `0.1.0-beta.5` in. But would be nice to know what's changed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-25 10:14:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1081" class=".btn">#1081</a>
            </td>
            <td>
                <b>
                    Encode custom width integers using the next power of two width
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Anchor IDL does not support custom width integers. Instead of creating a user-defined type for them, we will encode them using the smaller integer width greater than the given one.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 18:51:30 +0000 UTC
    </div>
</div>

