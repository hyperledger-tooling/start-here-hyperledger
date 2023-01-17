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
                PR <a href="https://github.com/hyperledger/solang/pull/1130" class=".btn">#1130</a>
            </td>
            <td>
                <b>
                    Refactor language server
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make the language server use a builder-style interface. Now, there is no need to pass the list of hovers around as a function argument.

This fixes the hover for destructure statements with variable definition, `a` in this example.

```solidity
contract c {
	function f() public {
		(int64 a) = (2);
	}
}
```

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-15 10:13:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1128" class=".btn">#1128</a>
            </td>
            <td>
                <b>
                    Refactor SCALE encoder into codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR makes the `AbiEncoding` trait more granular. This allowed me to move most of the logic into default implementations, leaving only a few `Type`s that needed to be handled differently in SCALE and Borsh. This means the Borsh and SCALE encoders can share most of their code :partying_face: 

The decoding side is untouched by this PR as it can be done independent. I will do it in a follow up PR, which will in turn allow to move the dispatcher out of emit into codegen as well. Which will finally allow to nuke the emit implementation of the SCALE encoder, as well as `substrace.c` from our stdlib.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 18:48:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1127" class=".btn">#1127</a>
            </td>
            <td>
                <b>
                    Update Rust version from workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The test workflows are failing because clap does not support Rust 1.63 anymore, so I updated it to 1.64.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 18:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1126" class=".btn">#1126</a>
            </td>
            <td>
                <b>
                    Differentiate between caller contract and the constructor contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When invoking `call_constructor` we were passing the same contract number for both the caller contract and the contract being called.

This fixes https://github.com/xermicus/fuzzy-sol/issues/118

The tests will only work after #1127 is merged.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 17:33:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1125" class=".btn">#1125</a>
            </td>
            <td>
                <b>
                    Use anchor npm library rather than @solana/solidity
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
        Created At 2023-01-11 15:31:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1124" class=".btn">#1124</a>
            </td>
            <td>
                <b>
                    Use match statements for comparison chains
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Lucas Steuernagel <lucas.tnagel@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 17:13:56 +0000 UTC
    </div>
</div>

