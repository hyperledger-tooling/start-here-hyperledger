---
layout: default
title: mirbft
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/mirbft
---

# mirbft <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/mirbft){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    Use new gRPC and Protobuf API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There code was still using the old Protobuf API,
while a recent protoc compiler was generating files using
the new one and, in some cases, did not even understand
the command-line options for gRPC.

All code now uses the new Protobuf API
and the generation commands (protos/generate.go) are fixed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 16:31:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    Fix data races and polish mircat
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
        Created At 2022-03-02 10:28:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    Fix missing defer in node.go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matej Pavlovic <matopavlovic@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 10:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/mirbft/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    Fix broken link in README, improve code doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matej Pavlovic <matopavlovic@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 10:32:41 +0000 UTC
    </div>
</div>

