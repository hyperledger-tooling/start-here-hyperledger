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
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    fix: MongoDB provider GetStoreConfig returning ErrStoreNotFound
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added a workaround for an issue where if you call OpenStore without having stored any data or created indexes, then the GetStoreConfig method will report ErrStoreNotFound. This is due to how MongoDB defers the creation of the underlying database until actual storage calls are made.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-12 20:23:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/241" class=".btn">#241</a>
            </td>
            <td>
                <b>
                    chore: update to latest orb revision
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
        Created At 2022-04-12 19:38:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/240" class=".btn">#240</a>
            </td>
            <td>
                <b>
                    chore: update to latest aries in sidetree vdr
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
        Created At 2022-04-12 18:47:32 +0000 UTC
    </div>
</div>

