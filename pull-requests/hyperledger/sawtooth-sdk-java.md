---
layout: default
title: sawtooth-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/sawtooth-sdk-java
---

# sawtooth-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/sawtooth-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/sawtooth-sdk-java/pull/42" class=".btn">#42</a>
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
        Created At 2021-10-05 16:09:27 +0000 UTC
    </div>
</div>

