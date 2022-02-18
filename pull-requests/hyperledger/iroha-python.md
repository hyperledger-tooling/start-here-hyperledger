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
                PR <a href="https://github.com/hyperledger/iroha-python/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Update proto files and generated python files to support Iroha 1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">iroha1</span>
            </td>
            <td>
                New features were added to https://github.com/hyperledger/iroha in version Iroha 1.4, which modified protobuf files. Thats why client libraries should be updated.

Features which modified protobuf files:
1. Syncing nodes: https://github.com/hyperledger/iroha/pull/1648/
2. Health check: https://github.com/hyperledger/iroha/pull/1735
_____________
- commit 1: I've updated proto files with attached script: https://github.com/hyperledger/iroha-python/blob/main/scripts/download-schema.py
- commit 2: I've generated python files from proto with attached script: https://github.com/hyperledger/iroha-python/blob/main/scripts/compile-proto.py
_____________
Signed-off-by: Grzegorz Bazior <g.bazior@yodiss.pl>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 13:45:00 +0000 UTC
    </div>
</div>

