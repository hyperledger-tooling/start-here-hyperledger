---
layout: default
title: blockchain-explorer
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.7
                </span>
            </td>
            <td>
                <!-- (SPDX-License-Identifier: CC-BY-4.0) -->  <!-- Ensure there is a newline before, and after, this line -->

## New Features

* None

## Bug Fixes and Updates

* [BE-876](https://jira.hyperledger.org/browse/BE-876) Stop unnecessary discovery request (#255)
* Bugfix: tailing ampersand sign prevents container from restarting (#254)
* [BE-857](https://jira.hyperledger.org/browse/BE-857) Change invoking function of lifecycle scc to allow non-admin client access (#252)
* Bugfix: timeout error crashing explorer (#253)
* Bugfix: disable enableAuthentication auth auto login using wrong network key issue (#250)

## Known Vulnerabilities

```
jsrsasign  <10.2.0
Severity: critical
RSA signature validation vulnerability - https://npmjs.com/advisories/1672
fix available via `npm audit fix --force`
Will install fabric-network@1.4.1, which is a breaking change
node_modules/jsrsasign
  fabric-ca-client  *
  Depends on vulnerable versions of fabric-common
  Depends on vulnerable versions of jsrsasign
  node_modules/fabric-ca-client
  fabric-common  >=2.1.1-snapshot.390
  Depends on vulnerable versions of jsrsasign
  node_modules/fabric-common
    fabric-network  >=1.4.19-snapshot.1
    Depends on vulnerable versions of fabric-common
    node_modules/fabric-network

4 critical severity vulnerabilities
```
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/blockchain-explorer/releases/tag/v1.1.7" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-07-05 08:15:19 +0000 UTC
    </span>
</div>

