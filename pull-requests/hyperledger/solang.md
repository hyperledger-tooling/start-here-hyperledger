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
                    LLVM 15 and v0.2.2 Release
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1157" class=".btn">#1157</a>
            </td>
            <td>
                <b>
                    Fix: typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix: typos

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-04 16:21:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1156" class=".btn">#1156</a>
            </td>
            <td>
                <b>
                    Retry uploading of program code after failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Uploading of program code intermittently fails, which causes CI tests to fail. Improve this a little bit.

Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 10:19:33 +0000 UTC
    </div>
</div>

