---
layout: default
title: fablo
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/fablo
---

# fablo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fablo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    1.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.1.0
                </span>
            </td>
            <td>
                ### Features
* Support Fabric Gateway since Fabric 2.4 [#305](https://github.com/hyperledger-labs/fablo/issues/305)
* Introduce pre-restore hook
* Attach `fabric-ca-server-config.yaml` as a volume [#168](https://github.com/hyperledger-labs/fablo/issues/168)
* Support tls for CA [#229](https://github.com/hyperledger-labs/fablo/issues/229)
* Use nvm to switch node version for chaincode build
* Allow to run peers in dev mode [#126](https://github.com/hyperledger-labs/fablo/issues/126)
* Allow to install each chaincode manually

### Fixes
* Support Apple M1 / arm64 architecture
* Various fixes in channel scripts
* Remove remaining docker containers and images after prune

### Chore & Maintenance
* Add `fabricNodeenvVersion` global configuration
* Update Node.js runtime compatibility ([details](https://github.com/hyperledger-labs/fablo/issues/274))
* Update legacy URLs

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/fablo/releases/tag/1.1.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-07-16 18:26:09 +0000 UTC
    </span>
</div>

