---
layout: default
title: sawtooth-sdk-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-python
---

# sawtooth-sdk-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-python/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Pin mistune version to fix doc build error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Sphinx-openapi depends on m2r which pulls in mistune without specifying a
version. Mistune has recently updated to 2.0.0 which includes some API
changes which were not backwards compatible.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 16:03:23 +0000 UTC
    </div>
</div>

