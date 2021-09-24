---
layout: default
title: firefly-tokens-erc1155
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc1155
---

# firefly-tokens-erc1155 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc1155){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/26" class=".btn">#26</a>
            </td>
            <td>
                <b>
                    Remove references to labs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 20:39:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc1155/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    Replace arbitrary "data" param on /pool with individual fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This has gone back and forth a few times, but it does seem like there's a
specific need for a "trackingId" that can be used to correlate the request with
the created pool, and that this is the only piece of extra data that needs to
be written to the chain.

Also adds a "config" parameter to the API - not used currently, but this
gives some future-proofing so it will be accepted and ignored by this version
of the connector if it is needed in the future.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-23 17:51:49 +0000 UTC
    </div>
</div>

