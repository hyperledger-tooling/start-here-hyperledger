---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3598" class=".btn">#3598</a>
            </td>
            <td>
                <b>
                    wip: pEx refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - pEx implementation no longer needs to replace Credential ID temporarily
- assorted cleanup
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 13:47:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3596" class=".btn">#3596</a>
            </td>
            <td>
                <b>
                    chore: improve stability of flaky tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add retry to mediator.Service.GetConnections
- add retry to ld/store.RemoteProviderStore.Save
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 19:53:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3595" class=".btn">#3595</a>
            </td>
            <td>
                <b>
                    Pull mathlib with support for 32-bit builds
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**

Pull mathlib with support for 32-bit builds

**Description:**

After the switch to [mathlib](https://github.com/IBM/mathlib/), builds on 32-bit platforms failed, owing to the fact that mathlib was using a version of [fabric-amcl](https://github.com/hyperledger/fabric-amcl) which didn't include 32-bit implementations. Pulling the latest mathlib fixes the issue.

**Summary:**

We just update all the `go.mod` to refer to the latest mathlib.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 15:27:57 +0000 UTC
    </div>
</div>

