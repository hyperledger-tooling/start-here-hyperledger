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
                PR <a href="https://github.com/hyperledger/firefly-evmconnect/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Improve handling of custom errors in receipts - capture returnValue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly/issues/1466 for details 

This PR is the first step of capturing the returnValue in cases it cannot be parsed as a default error
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 20:06:01 +0000 UTC
    </div>
</div>

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

