---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/628" class=".btn">#628</a>
            </td>
            <td>
                <b>
                    update node version to 20.15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When I upgraded node to 20.15 only, the following error is reported:

node:internal/crypto/hash:79
  this[kHandle] = new _Hash(algorithm, xofLen, algorithmId, getHashCache());
                  ^
The environment variable NODE_OPTIONS needs to be set manually to force Node.js to use OpenSSL's older APIs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-20 00:51:37 +0000 UTC
    </div>
</div>

