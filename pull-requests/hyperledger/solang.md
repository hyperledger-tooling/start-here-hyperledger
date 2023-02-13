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
                PR <a href="https://github.com/hyperledger/solang/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    Account for leading zeros in hex number literals size width
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Matching the behavior of `solc`.

Signed-off-by: xermicus <cyrill@parity.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 23:28:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1172" class=".btn">#1172</a>
            </td>
            <td>
                <b>
                    Update CODEOWNERS
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
        Created At 2023-02-10 19:32:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1170" class=".btn">#1170</a>
            </td>
            <td>
                <b>
                    Bump solang-parser for crate publish
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
        Created At 2023-02-10 08:52:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    Fix CSE bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @xermicus found a bug in common subexpression elimination while working on the SCALE decoder. This PR fixes the bug, but the fix is only palliative for it might not cover all possible cases.

The problem would be best solved implementing a correct version of partial redundancy elimination, which leverages the available expressions analysis (already available) and an anticipated expression analysis not only to detect common subexpressions, but to know where exactly to evaluate them. This solution, nevertheless, is too time consuming to code and will be easier to implement when we have a new IR with SSA.

More information about partial redundancy elimination can be found in the Chapter 9.5 of the book `Compilers: Principles, Techniques & tools`, second edition, from Monica S. Lam.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 21:07:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1167" class=".btn">#1167</a>
            </td>
            <td>
                <b>
                    Fix CSE unchecked operations bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @seanyoung found that the CSE pass was not differentiating checked and unchecked arithmetic expressions. This PR fixes this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 12:02:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1166" class=".btn">#1166</a>
            </td>
            <td>
                <b>
                    Fix --math-overflow flag and add tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - fix `--math-overflow` cli option
- add test for `--math-overflow`
- adds unchecked to the cfg printer 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 09:41:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1165" class=".btn">#1165</a>
            </td>
            <td>
                <b>
                    LLVM 15
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adapts emit to opaque pointers and removes all the pointer casts, which are not necessary anymore. These changes are essential for us to migrate to LLVM 15.

LLVM builds have been tested [here](https://github.com/LucasSte/solang/actions/runs/4128649851/jobs/7133349350).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-08 22:04:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1164" class=".btn">#1164</a>
            </td>
            <td>
                <b>
                    Add --contract and --output-meta CLI flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are needed for the anchor cli tools
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-08 16:13:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1163" class=".btn">#1163</a>
            </td>
            <td>
                <b>
                    Fix solang language-server --importmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1162
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-08 15:09:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1160" class=".btn">#1160</a>
            </td>
            <td>
                <b>
                    Allow mappings to be named (solc-0.8.18 feature)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/solang/issues/1159

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-07 19:04:00 +0000 UTC
    </div>
</div>

