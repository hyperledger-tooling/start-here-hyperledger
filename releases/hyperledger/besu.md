---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.1.0-RC4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.1.0-RC4
                </span>
            </td>
            <td>
                ## 22.1.0-RC4

### Additions and Improvements
- Updated besu-native to version 0.4.3 [#3331](https://github.com/hyperledger/besu/pull/3331)

### Download Links
[https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC4/besu-22.1.0-RC4.tar.gz](https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC4/besu-22.1.0-RC4.tar.gz)
SHA256 f1e34fddf4aad0d6699b38f6bdeff3799255d2c9bfdab0718f5f72bf90b56117
[https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC4/besu-22.1.0-RC4.zip](https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC4/besu-22.1.0-RC4.zip)
SHA256 f5a2dd72c164fd609963a9f1c3c9993632cf6b7eff85ce6cac95e444a53f2de4
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.1.0-RC4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-31 02:27:17 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.1.0-RC3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.1.0-RC3
                </span>
            </td>
            <td>
                ## 22.1.0-RC3
- Changing the order in which we traverse the word state tree during fast sync. This should improve fast sync during subsequent pivot changes.

### 22.1.0-RC3 Breaking Changes
- Removed deprecated hash variable `protected volatile Hash hash;` which was used for private transactions [#3110](https://github.com/hyperledger/besu/pull/3110)

### Additions and Improvements
- Genesis file parameter `blockperiodseconds` is validated as a positive integer on startup to prevent unexpected runtime behaviour [#3186](https://github.com/hyperledger/besu/pull/3186)
- Add option to require replay protection for locally submitted transactions [\#1975](https://github.com/hyperledger/besu/issues/1975)
- Update to block header validation for IBFT and QBFT to support London fork EIP-1559 [#3251](https://github.com/hyperledger/besu/pull/3251)
- Move into SLF4J as logging facade [#3285](https://github.com/hyperledger/besu/pull/3285)

### Bug Fixes
- Fix regression on cors-origin star value
- Fix for ethFeeHistory accepting hex values for blockCount
- Fix a sync issue, when the chain downloader incorrectly shutdown when a task in the pipeline is cancelled. [#3319](https://github.com/hyperledger/besu/pull/3319)

### Download Links
[https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC3/besu-22.1.0-RC3.tar.gz](https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC3/besu-22.1.0-RC3.tar.gz)
SHA256 fb521c64529b5d19cc8121f91a14087a89a814a83ea1f372f15c0ebdba01bb3a
[https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC3/besu-22.1.0-RC3.zip](https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.1.0-RC3/besu-22.1.0-RC3.zip)
SHA256 f0bcad0275f15078dad1dcb87f49e7c86d754e4346a06e8ac2f9a690c4b8c088

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.1.0-RC3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-01-26 00:53:51 +0000 UTC
    </span>
</div>

