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
                PR <a href="https://github.com/hyperledger/solang/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    Add casts for yul pointer to integer conversion and vice versa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                yul allows implicit conversion of pointers to integers and vice versa.

Fixes https://github.com/xermicus/fuzzy-sol/issues/79

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-20 12:49:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    Load value before shifting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The shift operations were not loading values before creating the respective LLVM-IR instruction. This PR fixes this and closes https://github.com/xermicus/fuzzy-sol/issues/38.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 21:01:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    Fix encoder for multidimensional dynamic arrays
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The example in the tests is the one of the cases I found in which we can use two dynamic dimensions in an array. The example helped me find various bugs in the way I was treating them in the encoder. This is also going to help @xermicus with his #1128 PR.

@xermicus You can decided whether to merge this PR or incorporate the change into your PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 19:51:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1131" class=".btn">#1131</a>
            </td>
            <td>
                <b>
                    mappings and arrays can also cause recursive struct fields
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes https://github.com/xermicus/fuzzy-sol/issues/31
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-18 15:29:57 +0000 UTC
    </div>
</div>

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

