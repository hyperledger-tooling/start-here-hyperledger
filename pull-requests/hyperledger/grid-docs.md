---
layout: default
title: grid-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid-docs
---

# grid-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/260" class=".btn">#260</a>
            </td>
            <td>
                <b>
                    Change `POSTGRES_HOST_AUTH_METHOD` to `trust`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes an authentication error in Schemaspy after the Postgres 14
release.

trust authorization is not recommended for deployed databases, but is
acceptable in this instance because the database is only being used to generate
schema for documentation purposes.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 20:47:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    Clarify gridd public key in Creating Splinter Circuits
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The previous version of this documentation contained punctuation that was
potentially confusing to users who are not familiar with the key format
that gridd is expecting.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 21:32:29 +0000 UTC
    </div>
</div>

