---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4355" class=".btn">#4355</a>
            </td>
            <td>
                <b>
                    Bump google.golang.org/grpc to 1.53.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Note that grpc 1.52.0 changed behavior of Dial(),
empty string can no longer be passed.
Therefore this PR also updates tests that passed empty string.

Also remove the go.mod `replace` for github.com/cespare/xxhash/v2,
it is no longer needed and the grpc update also updates github.com/cespare/xxhash/v2.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-08 21:02:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4352" class=".btn">#4352</a>
            </td>
            <td>
                <b>
                    policy update protection test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Issue #4331 

#### Type of change

- Bug fix
- Test update

#### Related issues

#4331 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-03 13:19:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4345" class=".btn">#4345</a>
            </td>
            <td>
                <b>
                    Release commit for v2.2.13
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.2.13.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-02 15:38:19 +0000 UTC
    </div>
</div>

