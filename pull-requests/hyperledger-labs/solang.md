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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/637" class=".btn">#637</a>
            </td>
            <td>
                <b>
                    Support skiping implicit type cast checking by using flag --no-implicit-type-cast-check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi,

I created this PR to resolve the issue reported in https://github.com/hyperledger-labs/solang/issues/632 where Solang reports errors on implicit type truncation of integers (which Solc can compile well).

In particular, I added a field `pub implicit_type_cast_check: bool` into the structure `Options` to capture this flag.

I also move the structure `Options` from `codegen/mod.rs` into `lib.rs` so that the compiler options can be accessed by both `sema` and `codegen` modules.

Can you review this PR and advise if my implementation can be merged?

Thank you!


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 09:59:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/636" class=".btn">#636</a>
            </td>
            <td>
                <b>
                    feat(parser): missing assembly statements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger-labs/solang/issues/631
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 12:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/635" class=".btn">#635</a>
            </td>
            <td>
                <b>
                    Enable linux arm64 build on self hosted runner
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
        Created At 2022-01-10 11:10:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/634" class=".btn">#634</a>
            </td>
            <td>
                <b>
                    feat(parser): try statements without low-level catch clause
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger-labs/solang/issues/633
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-09 13:52:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/630" class=".btn">#630</a>
            </td>
            <td>
                <b>
                    Add location to solidity import directive
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Pertaining to the discussion in [ethers-rs/feat(solc): flatten](https://github.com/gakonst/ethers-rs/pull/774) PR, add location to the import directives to be able to parse them out.

cc: @mattsse 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-08 15:19:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/628" class=".btn">#628</a>
            </td>
            <td>
                <b>
                    Update test.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 20:49:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/627" class=".btn">#627</a>
            </td>
            <td>
                <b>
                    Add slice to solidity parser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #626 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 10:41:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/624" class=".btn">#624</a>
            </td>
            <td>
                <b>
                    Fix regressions in ewasm after address type conversion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #623 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 10:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/622" class=".btn">#622</a>
            </td>
            <td>
                <b>
                    Improve subscript ast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - Track dereferenced type
 - Remove Expression::StorageBytesSubscript
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 22:12:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/621" class=".btn">#621</a>
            </td>
            <td>
                <b>
                    feat(parser): DocComments grouping & type annotation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger-labs/solang/issues/620

---

- [x] Differentiate different doc comment styles: line (`/// @author Alexey`) and block (`/** @author Alexey */`)
- [x] Group multiple block doc comments into one introducing `SingleDocComment` that's contained in `DocComment::Block` enum variant
- [x] Preserve newlines in both line and block doc comments, so it would be possible to restore the original formatting of comments
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 21:43:28 +0000 UTC
    </div>
</div>

