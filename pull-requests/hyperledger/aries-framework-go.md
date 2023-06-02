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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3593" class=".btn">#3593</a>
            </td>
            <td>
                <b>
                    feat: update jsongold
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                according to diff most changes are related to error handling, linter and optimizations.

initial reason for upgrade is https://github.com/piprate/json-gold/commit/c70834a618fd6c8f9202d23a851f578328cfec4b this change
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 10:33:13 +0000 UTC
    </div>
</div>

