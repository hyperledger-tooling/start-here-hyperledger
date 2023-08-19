---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/172" class=".btn">#172</a>
            </td>
            <td>
                <b>
                    Retry database file removal on windows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #167 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 19:41:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/171" class=".btn">#171</a>
            </td>
            <td>
                <b>
                    fix(js)!: use patched ref-napi/ffi-napi for nodejs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Similar approach as https://github.com/hyperledger/anoncreds-rs/pull/231 to make an easier set up in Node.js environment.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 19:16:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/170" class=".btn">#170</a>
            </td>
            <td>
                <b>
                    feat(js): use buffer instead of text-decoder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Do not depend on fast-decoding anymore
- added simple example app which can be used for testing.
  - NOTE: it is currently rather annoying to fully recompile aries-askar for all the android and iOS architectures so we would have to find a solution for that.

This is by no means a perfect app for testing and if we would rather wait for a better testing app I can remove it from this PR and create it later.

Ideally I would like to move to use `pnpm` as it makes dealing with workspaces a whole lot easier. And create some way to "quickly" (still need to compile askar like 6 times...) use custom askar builds.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 18:25:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    Add profile management and store export to JS wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently in draft because I can't build or test the react-native updates.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 16:57:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    fix(js): add p384 key algo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This simply adds a constant for P384 key algo support (added in #157) from JS. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 20:01:55 +0000 UTC
    </div>
</div>

