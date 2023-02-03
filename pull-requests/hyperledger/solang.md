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
                PR <a href="https://github.com/hyperledger/solang/pull/1155" class=".btn">#1155</a>
            </td>
            <td>
                <b>
                    Build fix after ink crate 4.0.0-rc was released
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
        Created At 2023-02-02 10:14:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1154" class=".btn">#1154</a>
            </td>
            <td>
                <b>
                    Substrate: Update integration test dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make the CI great again

Signed-off-by: xermicus <cyrill@parity.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 19:04:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1153" class=".btn">#1153</a>
            </td>
            <td>
                <b>
                    External function type should not be a pointer in `llvm_type` function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When we use the function `llvm_type`, it returns an llvm struct type for structs but a pointer for `Type::ExternalFunction`, which is also a struct in Solang emit. This behavior is inconsistent and gives us headaches when moving to LLVM 15.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 15:26:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1151" class=".btn">#1151</a>
            </td>
            <td>
                <b>
                    Bump some crate dependencies
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
        Created At 2023-02-01 14:17:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1150" class=".btn">#1150</a>
            </td>
            <td>
                <b>
                    Reporting runtime errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                runtime errors are reported alongside with file number and line number. this is enabled by ``--report-errors=true`
Signed-off-by: salaheldinsoliman <salaheldin_sameh@aucegypt.edu>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 02:27:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1149" class=".btn">#1149</a>
            </td>
            <td>
                <b>
                    Remove `Builtin::Random` completely
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since the depreciation in the Substrate runtime API we no longer have a use for that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 14:19:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1148" class=".btn">#1148</a>
            </td>
            <td>
                <b>
                    Substrate CI: Contract builder should use the same version as the contract node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Found another one...
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 13:00:18 +0000 UTC
    </div>
</div>

