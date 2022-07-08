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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    Examples refactor + added example of MST developed by Leo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">iroha1</span>
            </td>
            <td>
                I've refactored `tx-example.py` for now. The plan is to refactor rest of samples similar way.

I've also added MST example from Leo (@iptelephony): https://github.com/iptelephony/jubilant-engine with some modifications. He agreed:
![obraz](https://user-images.githubusercontent.com/15332594/177155900-d8ef1af8-9a20-4281-b071-f04db8f6e519.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 12:34:30 +0000 UTC
    </div>
</div>

