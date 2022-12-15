---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1101" class=".btn">#1101</a>
            </td>
            <td>
                <b>
                    Update roadmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Version 0.2 has already been released. It can be removed from the roadmap.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 22:07:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1100" class=".btn">#1100</a>
            </td>
            <td>
                <b>
                    Only emit in codegen when needed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes the need for `Expression::CodeLiteral` in codegen.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 16:54:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1099" class=".btn">#1099</a>
            </td>
            <td>
                <b>
                    Update `@solana/solidity.js` version to fix Solana integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #1089 introduced discriminators to replace selectors on Solana. This broke the integration tests and needed an updated version of our `@solana/solidity.js` Typescript library. This PR fix such an issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 20:25:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1097" class=".btn">#1097</a>
            </td>
            <td>
                <b>
                    Bugfix 1076: Destructing referenced types need a load
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #1076 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-11 17:53:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1096" class=".btn">#1096</a>
            </td>
            <td>
                <b>
                    msg.sender should not exist on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                Explanation in `docs/language/function.rst` 

- Remove  `msg.sender`
- Remove `caller` on yul
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 16:09:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1095" class=".btn">#1095</a>
            </td>
            <td>
                <b>
                    Use annotations for selectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">solana</span>
            </td>
            <td>
                Use the new annotations:

```
@selector([1,1,2,5])
function foo() {}
```
Rather than:
```
function foo() selector=hex"01010205" {}
```

This removes the old syntax completely.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 16:06:24 +0000 UTC
    </div>
</div>

