---
layout: default
title: firefly-evmconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-evmconnect
---

# firefly-evmconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-evmconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/111" class=".btn">#111</a>
            </td>
            <td>
                <b>
                    fixing copy right headers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                as per title
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 12:01:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Fix docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is an issue with building docker 

`ERROR: failed to solve: golang:1.21-buster: docker.io/library/golang:1.21-buster: not found`

https://github.com/hyperledger/firefly-evmconnect/actions/runs/7922199644/job/21629266487#step:11:156

Fixed it by using 1.21-alpine3.19 as for example for [tezos connector](https://github.com/hyperledger/firefly-tezosconnect/pull/34)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 10:46:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/109" class=".btn">#109</a>
            </td>
            <td>
                <b>
                    Propagate block number to eth_call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We had done the work to propagate through the `blockNumber` from FFTM, but not actually passed it down to the `eth_call` when specified.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 19:43:52 +0000 UTC
    </div>
</div>

