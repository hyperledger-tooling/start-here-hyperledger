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
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/205" class=".btn">#205</a>
            </td>
            <td>
                <b>
                    Integrate watcher into client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 11:46:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    Improve documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 11:43:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    Fix basic issue template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issue templates must have an about text.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 11:28:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    balance reader interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #200 

Introduces a balance reader interface for the generic client tests.

(Also moves `func makeRoleSetups` to a more suitable location.)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 10:51:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    Update and rename issue.md to basic.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When creating a new issue, the template description looked a bit odd. Hence, adjusting.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 10:43:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/198" class=".btn">#198</a>
            </td>
            <td>
                <b>
                    Integrate StatesPub into client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Prep step for integrating refactored watcher (for IoT) use cases.

Resolves #197.

Note: Only the last commit is relevant. Other commits are already part of another (PR #182).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-16 08:51:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Channel.Backend: Remove Params from Sign and Verify
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #195 #190 

Depends on #191 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 19:18:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    193 rename wallettest variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #193 

The variable name was suggesting that it can always be initialized with `Address.Bytes`, but the tests were assuming that the address is decodable, which is not necessarily true for `Address.Bytes`. In particular, note that the length of `Address.Bytes` can be retrieved using the `len` operator, while the length of an encoded address must either be known in advance or contained in the encoding.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 08:34:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    [channel/test] Generate modified params with correct id
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #189 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-15 07:10:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/187" class=".btn">#187</a>
            </td>
            <td>
                <b>
                    Create issue template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding a simple issue template
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 16:38:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    [pkg/test] Remove deprecated function.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `InterfaceData()` is deprecated and returns unreadable data in the
current go version. Use `Interface()` instead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 08:13:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/185" class=".btn">#185</a>
            </td>
            <td>
                <b>
                    Define smaller interfaces for methods in adjudcator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Previously, the adjudicator interface consisted of four methods.

- But, only some of the methods were required in any particular place.

- Hence, define an interface for each of the methods and compose the
  adjudicator interfaces from these smaller interfaces.

Resolves #184.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 19:09:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    [pkg/errors] Add Gatherer DoneOrFailed(Ctx)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #181  
Need this for testing, @RmbRT also seems to appreciate it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 18:24:46 +0000 UTC
    </div>
</div>

