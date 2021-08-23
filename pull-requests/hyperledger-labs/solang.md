---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    Minor fixes
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
        Created At 2021-08-22 17:59:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/470" class=".btn">#470</a>
            </td>
            <td>
                <b>
                    Update ci image from github actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 08:43:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/469" class=".btn">#469</a>
            </td>
            <td>
                <b>
                    Clippy fixes
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
        Created At 2021-08-20 15:45:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/468" class=".btn">#468</a>
            </td>
            <td>
                <b>
                    Implement undefined variable detection and prettify warning messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements undefined variable detection for variables in function scope, using the current reaching definitions implementation. A few points need further improvement:
1. Reaching definitions does not work across functions, which prevents us from detecting new definitions on function calls, whose arguments are memory references.
2. Codegen Instruction `Instr::AbiDecode` needs refactoring to make reaching definitions work properly with try-catch statements.

In addition, the PR prettifies warnings and errors messages Solang prints to CLI. Here is an example of the new formatting:
```
examples/test.sol:24:13-18: error: unreachable statement
Line 24:
	a = 5;
	^^^^^
```

This work is part of the Linux Foundation mentorship for the Hyperledge Solang compiler. For more information, please refer to the [project plan](https://wiki.hyperledger.org/display/INTERN/Project+plan+-+Solang+compiler+passes+2021).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 19:42:20 +0000 UTC
    </div>
</div>

