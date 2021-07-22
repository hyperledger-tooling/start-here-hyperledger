---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/indy-plenum/issues/1551" class=".btn">1551</a>
            </td>
            <td>
                <b>
                    Ubuntu 20.04: Upgrade RocksDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Ubuntu 20.04</span><span class="chip">help wanted</span><span class="chip">upgrade</span>
            </td>
            <td>
                For the Ubuntu 20.04 version of Plenum, upgrade to RocksDB 5.17, which is the version supported on Ubuntu 20.04; https://packages.ubuntu.com/search?searchon=sourcenames&keywords=rocksdb

Background:
- Plenum is currently dependent on RocksDB 5.8.8.
- When RocksDB 5.17 is used without any code changes several tests hang due to issues encountered by the code under test with the updated version of RocksDB.  See https://github.com/hyperledger/indy-plenum/issues/1546 for additional details.
- Therefore updates to the code are required to support RocksDB 5.17
- As an interim solution the RocksDB 5.8.8 package built by the `Build 3rd Party Dependencies` job (of the GHA Workflow) will be used.  Refer to https://github.com/hyperledger/indy-plenum/issues/1546#issuecomment-883585912 for details.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 14:39:19 +0000 UTC
    </div>
</div>

