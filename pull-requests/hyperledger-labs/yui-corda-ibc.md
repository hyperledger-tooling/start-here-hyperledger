---
layout: default
title: yui-corda-ibc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-corda-ibc
---

# yui-corda-ibc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-corda-ibc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-corda-ibc/pull/19" class=".btn">#19</a>
            </td>
            <td>
                <b>
                    Switch to ibc-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                close #17 

- Remove the Git submodule `external/cosmos-sdk`
- Use `ibc-go/proto` instead of `cosmos-sdk/proto` to auto-generate Kotlin/Rust codes
- Fix the Handler logic of `connOpenInit` and so on based on the implementation of `ibc-go` rather than the ICS spec
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 03:27:59 +0000 UTC
    </div>
</div>

