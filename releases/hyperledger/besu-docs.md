---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.1.0-RC2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.1.0-RC2
                </span>
            </td>
            <td>
                ## 22.1.0-RC2

### 22.1.0-RC2 Breaking Changes
- Removed deprecated hash variable `protected volatile Hash hash;` which was used for private transactions [#3110](https://github.com/hyperledger/besu/pull/3110)

### Additions and Improvements
- Re-order external services (e.g JsonRpcHttpService) to start before blocks start processing [#3118](https://github.com/hyperledger/besu/pull/3118)
- Stream JSON RPC responses to avoid creating big JSON strings in memory [#3076] (https://github.com/hyperledger/besu/pull/3076)

### Bug Fixes
- Make 'to' field optional in eth_call method according to the spec [#3177] (https://github.com/hyperledger/besu/pull/3177)
- Update to log4j 2.17.1. Resolves potential vulnerability only exploitable when using custom log4j configurations that are writable by untrusted users.


### Download Links
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC2/besu-22.1.0-RC2.zip 
 SHA256: 86c97c935d70857d210016eb73f518fddd5dcef0c7928c5ede4622bf62c69d17
- https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC2/besu-22.1.0-RC2.tar.gz 
SHA256 327c14e1829d39e65f822478b166519e781ac4714f54da39ba26d21ba5729a1e
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/22.1.0-RC2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-06 15:22:10 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    21.10.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    21.10.6
                </span>
            </td>
            <td>
                ## Bug Fixes
Update log4j to 2.17.1

## Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/21.10.6/besu-21.10.6.tar.gz SHA256 ef579490031dd4eb3704b4041e352cfb2e7e787fcff7506b69ef88843d4e1220
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/21.10.6/besu-21.10.6.zip SHA256 0fdda65bc993905daa14824840724d0b74e3f16f771f5726f5307f6d9575a719
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu-docs/releases/tag/21.10.6" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-12-21 21:20:11 +0000 UTC
    </span>
</div>

