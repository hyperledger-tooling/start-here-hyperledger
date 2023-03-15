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
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/144" class=".btn">#144</a>
            </td>
            <td>
                <b>
                    fix(js): defer library loading for nodejs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prevent native library from being loaded right when `@hyperledger/anoncreds-nodejs` is imported by deferring its loading to when it's actually used. 

This is a problem we found during AFJ test suites, which import the library in general purpose test helpers and make the native library to be loaded more times than needed, allocating more memory and making the suite to crash.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 16:52:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/142" class=".btn">#142</a>
            </td>
            <td>
                <b>
                    chore: update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated dependencies to their latest version
- Removed the dependency on openssl-src from github which should drastically
  increase first build times (also on CI)

Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-12 11:12:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    chore: set version to 0.1.0-dev.10
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
        Created At 2023-03-11 11:50:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    fix(js): strings in FFI structs and JSON conversion in react native
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixes `XXXFromJson()` functions that were losing the input string value due to the usage of vectors
- Fixes `createPresentation` and `verifyPresentation`, that were losing strings that were passed to FFI structures, and also were not being freed after usage
- Updates some methods like `createRevocationStatusList` and `verifyPresentation` according to last API changes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-10 00:13:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    fix: add support for legacy schema and cred def id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @genaris this should fix your issue regarding the invalid cred_def / schema identifiers.

I was wondering if anyone knows a regex to match the revocation registry definition id and the revocation registry id.

Since the new identifier checker checks if it's just a uri, we will validate incorrect schemas with a version of `3` for example. Curious to hear if we want to fix this or leave as-is.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-09 10:40:44 +0000 UTC
    </div>
</div>

