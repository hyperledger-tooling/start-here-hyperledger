---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Move pkg/io to wire/perunio
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Completes step 1.2 described in #233.

Regarding the choice of name for the package, I considered three options
1. `wire/io`: It doesn't convey that this is a custom serialization implementation done by perun team.
2. `wire/perun`: When using methods on the package, we will have to use `perun.Encode` or `perun.Decode`. I felt like, these methods have to do something with the perun project itself, not just serialization.
3. `wire/perunio`: This seems (to me) to solve both the above problems. So, I chose this name.

But, I am open to changing the name of the package if there is a better alternative.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 07:46:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    Use fixed length format for (un)marshalling asset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Previously, pkgio.(Encode|Decode) methods were used for
  marshallign/unmarshalling the Asset. This coupled the asset to a
  specific serialization implementation (pkg/io).

- Instead, use binary.BigEndian.Putuint64 directly.

Closes #283
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 07:40:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Introduce and use Asset.Equal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #247 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 14:14:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    log: Add comments to logger interfaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #262 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 12:47:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Lint comments on exported objects (functions, types, ...)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #267 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 12:23:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    Enable context check linter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #275 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 00:25:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    CI: Update workflow after changing from dev to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just a minor update to the CI workflow.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 21:19:44 +0000 UTC
    </div>
</div>

