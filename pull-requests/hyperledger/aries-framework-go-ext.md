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
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    fix: Return error when using duplicate tag names in MongoDB and CouchDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Put operations in the MongoDB and CouchDB operations that used the same tag name multiple times would result in all but the last usage getting lost due to the slice to map conversion that happens. With some effort, this issue may be fixable in the future, but for now I've updated the methods to return an explicit error to prevent unexpected behaviour.

Also updated golang.org/x/sys version in the mongodb module to resolve an issue when compiling with Go 1.18.

Also removed a TODO marker from the CouchDB implementation that is no longer needed.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 15:00:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/238" class=".btn">#238</a>
            </td>
            <td>
                <b>
                    chore: update to latest orb
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
        Created At 2022-04-12 09:11:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/237" class=".btn">#237</a>
            </td>
            <td>
                <b>
                    fix: postgres default db
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
        Created At 2022-04-11 14:55:30 +0000 UTC
    </div>
</div>

