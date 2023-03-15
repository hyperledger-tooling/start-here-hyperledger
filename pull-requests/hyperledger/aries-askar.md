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
                PR <a href="https://github.com/hyperledger/aries-askar/pull/122" class=".btn">#122</a>
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
                Prevent native library from being loaded right when `@hyperledger/aries-askar-nodejs` is imported by deferring its loading to when it's actually used. 

This is a problem we found during AFJ test suites, which import the library in general purpose test helpers and make the native library to be loaded more times than needed, allocating more memory and making the suite to crash.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-14 16:51:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    chore: update version
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
        Created At 2023-03-14 14:24:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/120" class=".btn">#120</a>
            </td>
            <td>
                <b>
                    feat(js): added migration to wrapper
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - chore: updated header and generation
- feat(js): indy-sdk to askar migration
- fix(js): fixed the nodejs tests
- test(js): added small migration tests and mock wallet

Sadly I had to copy the `.db` file instead of moving it in the test. For some very odd reason, which can be debugged later, if I moved it inside the tests I would get an `AEAD decryption error`. It is a slight overhead that should be fine for now.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-13 09:24:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/119" class=".btn">#119</a>
            </td>
            <td>
                <b>
                    fix(js): key handle name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There was a small inconsistency between the key handle name for `keyFree` between node.js and react native. As all other methods use `localKeyHandle` (which the RN also expected), i've changed the method and node implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-11 15:05:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/117" class=".btn">#117</a>
            </td>
            <td>
                <b>
                    Update version to 0.2.8
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
        Created At 2023-03-10 22:35:29 +0000 UTC
    </div>
</div>

