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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    Support immutable keyword
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 08:32:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/440" class=".btn">#440</a>
            </td>
            <td>
                <b>
                    Array codegen fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-18 10:16:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    Improve error messages and only generate abis for concrete contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-17 09:21:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    Load array subscript index from contract storage
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
        Created At 2021-07-16 11:08:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/437" class=".btn">#437</a>
            </td>
            <td>
                <b>
                    Check used variables in Load expression and length call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements the used variable detection for the `Load` expression and marks arrays as assigned when there is a `length` call. The latter is necessary to prevent array being removed from the intermediary representation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 17:47:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    Check used variables in delete statement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR detects used variables in a `delete` statement. This is a fix for the[ Unused variable detection PR](https://github.com/hyperledger-labs/solang/pull/429).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 20:35:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    Do not warning about unused public storage variable or shadowed event declarations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @LucasSte please review if you have the time
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 15:49:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/434" class=".btn">#434</a>
            </td>
            <td>
                <b>
                    Add detection of variables in builtin calls and function calls with gas and value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the detection of used variables in builtin calls (like transfer and send) and function calls with gas and value.
These cases were not covered in the [original PR](https://github.com/hyperledger-labs/solang/pull/429) that implements unused variable detection, thus Solang are detecting variables used in such cases as unused.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 21:45:34 +0000 UTC
    </div>
</div>

