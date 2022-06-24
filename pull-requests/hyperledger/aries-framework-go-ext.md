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
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    chore: update to latest orb and vct
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
        Created At 2022-06-23 09:31:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/266" class=".btn">#266</a>
            </td>
            <td>
                <b>
                    chore: update sidetree-core-go in sidetree vdr
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
        Created At 2022-06-23 09:16:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/264" class=".btn">#264</a>
            </td>
            <td>
                <b>
                    feat: Remove MongoDB BatchAsJSON method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Removed the BatchAsJSON method since the new BulkWrite method introduced in the previous commit can do the same thing but with more flexibility
* Added a clarification on the PrepareDataForBSONStorage helper function (which is intended to be used with BulkWrite).
* BulKWrite now returns a more accurate error message if an InsertOne model is being used.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-20 20:27:59 +0000 UTC
    </div>
</div>

