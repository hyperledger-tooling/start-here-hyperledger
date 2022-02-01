---
layout: default
title: fabric-sdk-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-node
---

# fabric-sdk-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-node/pull/549" class=".btn">#549</a>
            </td>
            <td>
                <b>
                    Main fix issue 548
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hey folks, this is a rolling PR for now as I still need to write a proper test for this and actually run it locally.. 

So far I have just adapted some of what I monkey-patched the JS with to get it done with some additional TS goodies.

I created an additional TS definition for the constant `commitResponse` (`CommitResponse`) which helps provide a pretty clean solution to the potential problem where `commitResponse` is undefined as outlined in my recently filed issue #548.

Update: set to draft status for now to reflect its state.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 19:47:36 +0000 UTC
    </div>
</div>

