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
                PR <a href="https://github.com/hyperledger/iroha-deploy/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Add RocksDB support.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adding:
- RocksDB setup support
iroha_new_database_config is adding [new config of database definition](https://iroha.readthedocs.io/en/develop/configure/index.html#deployment-specific-parameters)
True - generate new config
False - stay with old parameter pg_opt (default value)

iroha_use_rdb it switcher between postgres and rdb in new type of database definition. Addition if it True will create volume with rdb files

- Possible to run Iroha container in priviledged mode if iroha_docker_priviledged=True

Tested by:
- [False value](https://jenkins.soramitsu.co.jp/job/qa/job/iroha1/job/iroha-dev/158/parameters/)
- [True value](https://jenkins.soramitsu.co.jp/job/qa/job/iroha1/job/iroha-dev/157/parameters/)
- [From master branch](https://jenkins.soramitsu.co.jp/job/qa/job/iroha1/job/iroha-dev/162/parameters/)

Signed-off-by: Stepan Lavrentev <lawrentievsv@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 11:22:50 +0000 UTC
    </div>
</div>

