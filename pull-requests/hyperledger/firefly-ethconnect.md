---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    Fix post-merge build issue related to error codes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See failure here https://github.com/hyperledger/firefly-ethconnect/runs/4301810830?check_suite_focus=true

Combination of #178 post-merge with #177

```
# github.com/hyperledger/firefly-ethconnect/internal/contractgateway
internal/contractgateway/smartcontractgw.go:529:31: undefined: "github.com/hyperledger/firefly-ethconnect/internal/errors".New
make: *** [Makefile:43: deps] Error 2
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 16:56:38 +0000 UTC
    </div>
</div>

