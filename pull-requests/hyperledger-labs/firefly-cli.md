---
layout: default
title: firefly-cli
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly-cli/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Improve ganache healthcheck and shorten timeouts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds an extra step to the ganache healthcheck, using `grep` to make sure that we actually get an HTTP upgrade response for the websocket. The previous code just assumed that if it didn't exit immediately that it was successful, which is not always a safe assumption. This also allows us to shorten the timeouts a bit, which should shave a few seconds off the stack startup time.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-16 13:40:44 +0000 UTC
    </div>
</div>

