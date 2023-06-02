---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/70" class=".btn">#70</a>
            </td>
            <td>
                <b>
                    feat: Add nested array config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of another feature I want to be able to add nested arrays such as:
```
namespaces:
  predefined:
  - name: myns
    tlsConfigs:
    - name: myconfig
      tls:
        enabled: true
```

This is not currently possible and this PR adds that support. Let me know if I missed out on anything!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 10:58:02 +0000 UTC
    </div>
</div>

