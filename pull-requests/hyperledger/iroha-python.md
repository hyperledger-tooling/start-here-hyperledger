---
layout: default
title: iroha-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-python
---

# iroha-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Generated protobuf files with protobuf 3.12.4 on Ubuntu 21.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">iroha1</span>
            </td>
            <td>
                This PR is to fix the issue:
https://github.com/hyperledger/iroha-python/issues/102

but first I need to check if code is working better:
```
pip3 install "git+https://github.com/baziorek/iroha-python.git@generate_protobufs_again"
```
after I'm sure that it is better code I'll change into normal PR instead of draft PR.

Signed-off-by: G.Bazior <bazior@agh.edu.pl>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 20:00:08 +0000 UTC
    </div>
</div>

