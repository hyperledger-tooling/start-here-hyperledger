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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    Update dependencies
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
        Created At 2021-12-31 11:30:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Make solidity parser a standalone crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is essentially a followup on #597 and makes the solidity parser a standalone crate (`solang-parser`)

## Changes
* move `src/parser/*` to `solang-parser`, including lalrpop build
* move `src/sema/ast/Diagnostic` related structs to `solang-parser/src/diagnostics/`. This was necessary because the parser's error is the Diagnostic, but has the downside that some `Diagnostic` implementation is now in two places:
  * made `src/sema/ast/Diagnostic::formatted_message` a function that accepts a `&Diagnostic` instead
* rm unused dependencies in solang 
* reexport the parser, so it doesn't break
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-30 19:45:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/614" class=".btn">#614</a>
            </td>
            <td>
                <b>
                    Add bytes buffer functions for encoding and decoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
contract c {
	function f() public returns (bytes) {
		bytes data = new bytes(10);
		data.writeUint32LE(102, 0);
		data.writeUint64LE(0xdeadcafe, 4);
		return data;	
	}
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-28 15:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    Builtin cleanups
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
        Created At 2021-12-27 12:22:18 +0000 UTC
    </div>
</div>

