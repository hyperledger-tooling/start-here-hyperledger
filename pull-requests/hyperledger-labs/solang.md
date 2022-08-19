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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/963" class=".btn">#963</a>
            </td>
            <td>
                <b>
                    add shell completions for cli app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a `shell-complete` sub-command, allowing users to autocomplete our CLI with the TAB key (this pretty much defuses the issue of typing full length sub-commands out all the time). As a bonus It also shows remaining options when there is nothing to complete yet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-14 13:20:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/961" class=".btn">#961</a>
            </td>
            <td>
                <b>
                    Create abi.borshDecode method for Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements Borsh Decoding and connects it to an experimental function called `abi.borshDecode` that only works for Solana. Using this function raises a compiler warning to inform the user that the borsh encoding is not completely supported yet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 20:38:07 +0000 UTC
    </div>
</div>

