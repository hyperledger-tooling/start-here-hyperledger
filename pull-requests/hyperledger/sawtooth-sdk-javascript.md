---
layout: default
title: sawtooth-sdk-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-javascript
---

# sawtooth-sdk-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-javascript/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    Remove `coverage` from test Dockerfiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The 6.0 release of Coverage dropped support for python 3.5, which is the last
supported version on Xenial so it can no longer be installed properly. However,
it's not required to run the tests so it can be removed safely.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 15:57:48 +0000 UTC
    </div>
</div>

