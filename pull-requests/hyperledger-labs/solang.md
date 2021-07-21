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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/446" class=".btn">#446</a>
            </td>
            <td>
                <b>
                    Ensure that enherited functions are also added to the abi file
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
        Created At 2021-07-21 14:50:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/445" class=".btn">#445</a>
            </td>
            <td>
                <b>
                    Ensure create contract works on Solana v1.7.3 and later
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
        Created At 2021-07-21 09:47:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/444" class=".btn">#444</a>
            </td>
            <td>
                <b>
                    Generate wasm and contract file for Substrate and other fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #443 

I think @athei asked for this feature too
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 09:09:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/442" class=".btn">#442</a>
            </td>
            <td>
                <b>
                    Improve warnings generated for incorrect function mutability
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
        Created At 2021-07-20 07:29:16 +0000 UTC
    </div>
</div>

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

