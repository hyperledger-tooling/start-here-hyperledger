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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/671" class=".btn">#671</a>
            </td>
            <td>
                <b>
                    Testcase for issue #666
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See issue #666 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-16 11:58:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/667" class=".btn">#667</a>
            </td>
            <td>
                <b>
                    Hyperledger chat has moved
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
        Created At 2022-02-15 18:40:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/664" class=".btn">#664</a>
            </td>
            <td>
                <b>
                    Permit error keyword to be used as variable name and ensure parser tests are run
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @shekhirin this might be of interest.

* The solang-parser crate tests were not being run
* Allow variable names to be `error` even though its a keyword
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 16:28:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/663" class=".btn">#663</a>
            </td>
            <td>
                <b>
                    Bump dependencies
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
        Created At 2022-02-11 09:23:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/662" class=".btn">#662</a>
            </td>
            <td>
                <b>
                    feat(parser): add support for custom error types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add
* ErrorDefinition
* ErrorParameter

support in lalrpop and ast types (based on existing EventDef/EventParam), following https://docs.soliditylang.org/en/v0.8.11/grammar.html#a4.SolidityParser.errorDefinition


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 17:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/661" class=".btn">#661</a>
            </td>
            <td>
                <b>
                    Fix line comments that end in non-ascii character
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The lexer assumed the last character was 1 byte.

Fixes #660 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 10:25:15 +0000 UTC
    </div>
</div>

