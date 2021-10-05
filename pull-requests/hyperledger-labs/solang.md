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
                PR <a href="https://github.com/hyperledger-labs/solang/pull/511" class=".btn">#511</a>
            </td>
            <td>
                <b>
                    Improve error message when accessing contract variable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 If a contract variable is not constant and it is accessed via the contract type, rather than a contract instance, give a nicer error message.
    

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 09:39:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/510" class=".btn">#510</a>
            </td>
            <td>
                <b>
                    Add support for destructive expressions in return
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ivan Waitusenok <sleepplease@protonmail.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 22:04:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/509" class=".btn">#509</a>
            </td>
            <td>
                <b>
                    Fix mixing variables with constants in contracts
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
        Created At 2021-10-04 19:09:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    Allow calling constants from contracts as well
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Iwan Waitusenok <sleepplease@protonmail.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 17:14:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/507" class=".btn">#507</a>
            </td>
            <td>
                <b>
                    Resolve constants from libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Iwan Waitusenok <sleepplease@protonmail.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-04 14:18:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/506" class=".btn">#506</a>
            </td>
            <td>
                <b>
                    The link to the llvm libraries on github is incorrect
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
        Created At 2021-10-02 16:25:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/505" class=".btn">#505</a>
            </td>
            <td>
                <b>
                    Resolve BytesLiteral to String when hinted
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Iwan Waitusenok <sleepplease@protonmail.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-01 16:30:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/504" class=".btn">#504</a>
            </td>
            <td>
                <b>
                    Generate LoadStorage instructions on related casts
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
        Created At 2021-09-30 11:30:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/503" class=".btn">#503</a>
            </td>
            <td>
                <b>
                    Implement available expression analysis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements an available expression analysis for the control flow graph of Solang. This analysis is going to be necessary for the common subexpression elimination pass to be implemented.

This PR is part of the Linux mentorship. For more information, please refer to the [project's wiki](https://wiki.hyperledger.org/display/INTERN/Project+plan+-+Solang+compiler+passes+2021).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-30 00:58:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/502" class=".btn">#502</a>
            </td>
            <td>
                <b>
                    Add value to solidity instruction on Solana
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Actual transfers not implemented yet, that will come in a following pr
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-29 11:19:16 +0000 UTC
    </div>
</div>

