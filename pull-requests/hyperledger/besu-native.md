---
layout: default
title: besu-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-native
---

# besu-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-native/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    disable blake tests on arm64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since the native blake2bf implementation is slower than the java implementation on arm64, it is not being built:
https://github.com/hyperledger/besu-native/blob/main/build.sh#L69-L76

Ignore this test if we are running on arm64.  Tested on OSX
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 20:21:57 +0000 UTC
    </div>
</div>

