---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    Add Reorg to SimulatedBackend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduces a `Reorg` function. Example can be found in #105.  
Im not quite sure here with the testing, if it is too complicated, we could leave it for later.  
  
It sadly uses a replace in the `go.mod`, lets see if it works in the CI.

Closes #105 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 14:59:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Add Auto-mining to SimulatedBackend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Introduces two functions: `StartMining(interval)` and `StopMining`.  
Can be used to simulate a ticking blockchain.  

Closes #103 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 13:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    Confirm TX with Finality Depth
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #97 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 18:23:36 +0000 UTC
    </div>
</div>

