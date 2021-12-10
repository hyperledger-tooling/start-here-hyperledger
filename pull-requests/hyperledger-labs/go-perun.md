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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/291" class=".btn">#291</a>
            </td>
            <td>
                <b>
                    Client: Adapt ForceUpdate to Update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #290 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 16:26:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/289" class=".btn">#289</a>
            </td>
            <td>
                <b>
                    💥 Rename `Channel.Update`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #288 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 14:47:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/287" class=".btn">#287</a>
            </td>
            <td>
                <b>
                    Merge perunio/test into wire/test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Completes step 1.3 described in #233.

This is done in two steps:

1. In the first step, the test helper function `TestMsg` which runs a set of generic tests on Msg is moved to perunio/test, where the other generic tests are located.

2. In the second step, the package "perunio/test" which contains test helpers for running various kinds of generic tests is merged into wire/test.

Details of the individual changes have been documented in the commit message.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-09 07:20:25 +0000 UTC
    </div>
</div>

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

