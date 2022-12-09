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
                PR <a href="https://github.com/hyperledger/solang/pull/1094" class=".btn">#1094</a>
            </td>
            <td>
                <b>
                    Add voting ballot example
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While I was searching for some good example to use in the blog post, I came across [this ballot example](https://docs.soliditylang.org/en/v0.8.17/solidity-by-example.html?highlight=comments#voting). It compiles without any warnings for Substrate and Solana. How do you feel about adding it?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 10:32:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1093" class=".btn">#1093</a>
            </td>
            <td>
                <b>
                    Smol README bugfix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Cyrill Leutwiler <cyrill@parity.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 15:42:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1092" class=".btn">#1092</a>
            </td>
            <td>
                <b>
                    Fix github actions warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Every CI run we get tons of warnings like:

The `set-output` command is deprecated and will be disabled soon. Please upgrade to using Environment Files.

It looks like actions-rs/toolchain is unmaintained:

https://github.com/actions-rs/toolchain/issues/221

Many projects are switching over to dtolnay/rust-toolchain, let's do the same.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 14:45:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1091" class=".btn">#1091</a>
            </td>
            <td>
                <b>
                    Ensure that rational compares are not permitted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This solidity was not rejected and causes a panic in emit, because rationals should be compile-time constants.

```
function foo1(uint64 a, uint64 b) returns (bool) {
	return (a/b) >= 0.05;
}
```

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 09:21:10 +0000 UTC
    </div>
</div>

