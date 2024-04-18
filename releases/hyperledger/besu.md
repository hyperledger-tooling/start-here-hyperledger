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
                    24.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    24.3.3
                </span>
            </td>
            <td>
                # 24.3.3 - P2P Blob Transaction Hotfix

24.3.3 is a **recommended hotfix** for mainnet, sepolia and holesky users, especially if your peer numbers are currently low.

- Fix to avoid broadcasting full blob txs which can cause peers to disconnect (particularly Geth) (https://github.com/hyperledger/besu/pull/6835)

**Full Changelog**: https://github.com/hyperledger/besu/compare/24.3.0...24.3.3

Note: 24.3.1 and 24.3.2 were skipped due to a bug in the release process.
Release 24.4.0 is still being worked on.

## Download Info
446ae8b42f71c02d413c64e5525aded31ee4925be7ef0c729ac1b374e805928b  besu-24.3.3.tar.gz
b44951e68c6978de7f289ebd5f0111f0087cd266fd0c133afcf33b2004aa1a2a  besu-24.3.3.zip

### Docker 

`docker pull docker.io/hyperledger/besu:24.3.3`

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/24.3.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-04-11 06:03:38 +0000 UTC
    </span>
</div>

