---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/301" class=".btn">#301</a>
            </td>
            <td>
                <b>
                    status code in IrohaClientException
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: akostiucenko <kostiuchenko@soramitsu.co.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-22 12:07:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    fix "bind: address already in use"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - findFreePorts function fixed by adding socket timeout (to not use port after all tests are done)
- containers initialize before anything (need to make `containers` property initialized in IrohaTest earlier the `@BeforeEach` method called)

Signed-off-by: akostiucenko <kostiuchenko@soramitsu.co.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 15:10:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    move network initialization to IrohaTest class
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: akostiucenko <kostiuchenko@soramitsu.co.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 12:39:21 +0000 UTC
    </div>
</div>

