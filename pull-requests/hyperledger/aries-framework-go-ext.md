---
layout: default
title: aries-framework-go-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go-ext
---

# aries-framework-go-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/166" class=".btn">#166</a>
            </td>
            <td>
                <b>
                    test: Update common tests and interface version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Latest common storage tests commit includes new tests.
- Updated MySQL implementation to pass them. The MySQL implementation also now defers creating a tag map until needed. It also now doesn't require SetStoreConfig in order to do queries in order to keep in line with the latest interface documentation.
- Updated some documentation for the CouchDB implementation.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-20 21:18:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/165" class=".btn">#165</a>
            </td>
            <td>
                <b>
                    feat: Reuse MongoDB connection across stores
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reworked the MongoDB storage provider to use one client (and one connection) across stores. It's safe to reuse that client object and saves on extra unnecessary connections.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 02:03:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    fix: allow creating docs with base58 keys in orb vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 22:10:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/163" class=".btn">#163</a>
            </td>
            <td>
                <b>
                    chore: update orb vdr to latest sidetree vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 19:39:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/162" class=".btn">#162</a>
            </td>
            <td>
                <b>
                    fix: allow creating/updating doc with base58 pub keys in vdr/sidetree
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 18:10:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/161" class=".btn">#161</a>
            </td>
            <td>
                <b>
                    docs: Fix incorrect MongoDB provider documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 15:01:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/160" class=".btn">#160</a>
            </td>
            <td>
                <b>
                    updated indy vdr component to be compliant with v0.1.6 aries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Suggestions and comments (including critiques) are more than welcomed. 

Signed-off-by: Ardian <ardianabazi09@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 16:13:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/159" class=".btn">#159</a>
            </td>
            <td>
                <b>
                    chore: add timeout for http client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Firas Qutishat <firas.qutishat@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 15:25:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/158" class=".btn">#158</a>
            </td>
            <td>
                <b>
                    chore: update AFGO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 15:12:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/156" class=".btn">#156</a>
            </td>
            <td>
                <b>
                    chore: update AFGO for sidetree vdr
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andriy Holovko <andriy.holovko@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 12:37:59 +0000 UTC
    </div>
</div>

