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
                PR <a href="https://github.com/hyperledger/solang/pull/1090" class=".btn">#1090</a>
            </td>
            <td>
                <b>
                    Release v0.2 TBD
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
        Created At 2022-12-02 08:32:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1089" class=".btn">#1089</a>
            </td>
            <td>
                <b>
                    WIP: Use discriminators on Solana instead of selectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lucas Steuernagel <lucas.tnagel@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 21:45:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1088" class=".btn">#1088</a>
            </td>
            <td>
                <b>
                    Freeze Borsh library version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `@dao-xyz/borsh` library had an update with breaking changes. This PR freezes the version that currently works with our Typescript tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 19:23:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1087" class=".btn">#1087</a>
            </td>
            <td>
                <b>
                    Add basic `ink!` to solidity call integration test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">substrate</span>
            </td>
            <td>
                My original plan was to hack the substrate emit phase to always return a `Result` type (`Ok` variant which is just a single null byte), so that the `LanguageError` from `ink!` version 4 is respected when calling a solidity contract from `ink!`. But while doing so I realized: Currently the only way to call a solidity contract from `ink!` is to use the low level `CallBuilder` interface anyways. And since this interface does not care at all about the `LanguageError`, everything still works. So now, instead of hacking around in emit and holding up the next solang release, I'd rather implement the `LanguageError` story cleanly after the release (IIRC it means refactoring the scale encoder into codegen and then implementing the `Result` type).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 15:32:12 +0000 UTC
    </div>
</div>

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

