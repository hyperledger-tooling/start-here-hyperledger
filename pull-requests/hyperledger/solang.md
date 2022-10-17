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
                PR <a href="https://github.com/hyperledger/solang/pull/1039" class=".btn">#1039</a>
            </td>
            <td>
                <b>
                    Implement more constructor dispatch in cfg
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
        Created At 2022-10-14 16:27:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1038" class=".btn">#1038</a>
            </td>
            <td>
                <b>
                    Encode arguments for constructor call in codegen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presently, when we call a constructor, we encode the arguments in emit, using the deprecated EthAbi encoding. A prior step to moving to Borsh is encoding all arguments during codegen. This PR refactors the `Instr::Constructor` to accommodate such changes, alongside the necessary adaptations in emit and codegen.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-13 17:04:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1037" class=".btn">#1037</a>
            </td>
            <td>
                <b>
                    Arrays whose elements are dynamic should be properly Borsh decoded
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When we try to decoded a fixed array whose type is dynamic, we cannot validate the buffer length before fetching more information about each element. I found this bug while migrating the Solana target to Borsh encoding.

This PR fixes this bug.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-10 20:17:19 +0000 UTC
    </div>
</div>

