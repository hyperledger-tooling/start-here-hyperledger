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
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    feat: Changes to MongoDB custom method parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changed the MongoDB CustomQuery method's filter parameter to be an interface{} to match the type used by the underlying driver. This allows the caller more flexibility in their queries.

Changed the MongoDB CustomQuery method's return parameter to be the specific MongoDB Iterator object instead of the storage interface's iterator type so that the caller can directly use the ValueAsRawMap method without doing a type assertion.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-27 00:45:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    feat: Added find options to MongoDB CustomQuery method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will give the caller the ability to have more control over custom queries in MongoDB.

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 18:54:03 +0000 UTC
    </div>
</div>

