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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    Replace dep on fftm+core with new firefly-common package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We ended up pulling in a huge tree of dependencies  by the definitions for the FFCAPI being FireFly Transaction Manager, which depends then on FireFly Core for types. Now everything has moved to FireFly Common, we have a much slimmer set of deps to pull in.

Also renamed `ffc` package to `ffcapiconnector` on feedback that `ffc` was too vague.

Depends on (go.mod pulls these in directly):
- https://github.com/hyperledger/firefly-common/pull/4
- https://github.com/hyperledger/firefly/pull/791

Also see:
- https://github.com/hyperledger/firefly-transaction-manager/pull/6
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 01:47:29 +0000 UTC
    </div>
</div>

