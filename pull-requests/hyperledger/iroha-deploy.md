---
layout: default
title: iroha-deploy
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-deploy
---

# iroha-deploy <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-deploy){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-deploy/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Add remove peer in python script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Changes
In some cases, it is easier to use docker image instead of Iroha cli.I updated the script to be able to un basic tasks.

## Examples
Add peer:
```
docker run -it \
  -e DEBUG=TRUE \
  -e IROHA_HOSTS=10.0.0.3:50051 \
  -e IROHA_ACCOUNT=admin@test  \
  -e IROHA_ACCOUNT_KEYS=f101537e319568c765b2cc89698325604991dca57b9716b58016b253506cab70 \
  soramitsu/iroha-docker-iroha-python:51a6648 \
   add_peer iroha-5:10001 f715eea67c27d507aee4923c8a7d622d5c1d5a79c0c5a2b7a4c8dcb5d492d912
 ```
 Remove peer
```
docker run -it \
  -e DEBUG=TRUE \
  -e IROHA_HOSTS=10.0.0.3:50051 \
  -e IROHA_ACCOUNT=admin@test  \
  -e IROHA_ACCOUNT_KEYS=f101537e319568c765b2cc89698325604991dca57b9716b58016b253506cab70 \
  soramitsu/iroha-docker-iroha-python:51a6648 \
   remove_peer f715eea67c27d507aee4923c8a7d622d5c1d5a79c0c5a2b7a4c8dcb5d492d912
```
## Author 
Signed-off-by: Bulat Saifullin <bulat@saifullin.ru>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 19:38:11 +0000 UTC
    </div>
</div>

