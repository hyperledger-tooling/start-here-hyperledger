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
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    fix: Use tags prefix only if not using raw JSON
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Bob Stasyszyn <Bob.Stasyszyn@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-09 19:03:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    chore: Return an interface from QueryCustom instead of struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Returning an interface from QueryCustom so that it's easier for clients to mock out the iterator in unit tests.

Signed-off-by: Bob Stasyszyn <Bob.Stasyszyn@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 22:00:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go-ext/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    feat: Added GetBulkAsRawMap function to the MongoDB API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                GetBulkAsRawMap returns a slice of 'raw' maps, one for each of the specified keys.

Also exposed PrepareFilter and CreateMongoDBFindOptions so that clients may prepare queries for use with the QueryCustom function.

Signed-off-by: Bob Stasyszyn <Bob.Stasyszyn@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-08 17:17:39 +0000 UTC
    </div>
</div>

