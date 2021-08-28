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
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    chore: Store JSON strings as string instead of binary in MongoDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A JSON string (e.g. ["text"]) is persisted as a string value instead of a binary value.

Also, collapse the data wrappers into one wrapper that can store binary, JSON documents, and strings.

Signed-off-by: Bob Stasyszyn <Bob.Stasyszyn@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-26 15:17:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    feat: GetStoreConfig can now be used to check for underlying database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the MongoDB implementation of GetStoreConfig to check for the underlying database's existence instead of looking at the in-memory store objects, per the storage interface documentation.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 21:50:17 +0000 UTC
    </div>
</div>

