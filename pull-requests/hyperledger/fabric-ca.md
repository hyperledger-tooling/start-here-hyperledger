---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    [WIP] Use bccsp instead of directly idemix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Part I: Migration and tests in lib/server/idemix work.

fabric-ca's usage of the idemix package(s) is incorrect. Instead of relying on the bccsp abstraction, it makes direct use of the low-level API and so makes it hard to switch implementations.

#### Type of change

Improvement (improvement to code, performance, etc)

#### Description

This PR switches to using idemix's bccsp abstraction.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-14 07:51:36 +0000 UTC
    </div>
</div>

