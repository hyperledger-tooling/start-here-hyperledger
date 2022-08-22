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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/983" class=".btn">#983</a>
            </td>
            <td>
                <b>
                    Always run linux arm64 tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Thanks for Hyperledger, we now have an mac m1 running asahi linux which we can use for linux arm64 tests and builds.

Now also run the tests on pull requests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 11:17:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/982" class=".btn">#982</a>
            </td>
            <td>
                <b>
                    Dev
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Multiplication overflow detection for bits > 64.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 08:13:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/981" class=".btn">#981</a>
            </td>
            <td>
                <b>
                    Remove ewasm target and rename usable parts for evm target
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Ethereum Foundation has stopped funding for ewasm work, so it is
unlikely to happen in the current form. In addition, burrow has been end
of life'd by Hyperledger. So, the ewasm target is no longer useful.

We would love to have an evm target at some point in the future. Many
parts of the ewasm target is re-usable for evm, so we rename ewasm to
evm and remove the parts which are irrelevant for evm.

Note that the new evm target is good enough for the language server, so
the language server can be started in evm mode:

```
solang language-server --target evm
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 16:42:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/980" class=".btn">#980</a>
            </td>
            <td>
                <b>
                    Make lexer public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Exposing the lexer API would be useful for things like syntax highlighting. Plus its implemented clean as is to be exposed directly :hugs: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 16:05:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/979" class=".btn">#979</a>
            </td>
            <td>
                <b>
                    Debug info patch - Fix #967
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix #967 to generate debug information with bitcode
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 10:39:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/968" class=".btn">#968</a>
            </td>
            <td>
                <b>
                    Introduce new syntax for overriding selector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This introduces syntax like so:
```
function get_foo() selector=hex"01020304" public return (int) {
    return 102;
}
```
Note this functionality will be used in a following commit to define interfaces derived from anchor idl files. Tests or Solana will be in that PR, no changes as the functionality will change in that PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 10:19:19 +0000 UTC
    </div>
</div>

