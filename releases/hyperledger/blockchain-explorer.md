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
                    v1.1.8
                </span>
            </td>
            <td>
                <!-- (SPDX-License-Identifier: CC-BY-4.0) -->  <!-- Ensure there is a newline before, and after, this line -->

## New Features

* None

## Bug Fixes and Updates

* BE-880 Fix incorrect multi-process logging (#260)
* docs: add code snippet for admin cert modification (#257) (#258)

## Known Vulnerabilities

package-lock.json
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
```

client/package-lock.json
```

```
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/blockchain-explorer/releases/tag/v1.1.8" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2021-08-16 13:49:20 +0000 UTC
    </span>
</div>

