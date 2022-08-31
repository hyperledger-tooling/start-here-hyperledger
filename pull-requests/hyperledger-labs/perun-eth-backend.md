---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-eth-backend/pull/33" class=".btn">#33</a>
            </td>
            <td>
                <b>
                    CI: Generate Binding: Use `git diff` instead of `go test`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously we used `go test` to check if the bindings were generated correctly. However, this always takes some time. Instead we now use `git diff` to test that the binding was rebuild correctly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-31 13:19:27 +0000 UTC
    </div>
</div>

