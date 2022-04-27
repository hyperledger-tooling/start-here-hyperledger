---
layout: default
title: firefly-ethconnect
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-ethconnect
---

# firefly-ethconnect <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-ethconnect){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    Fix release GitHub action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 17:52:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    Intermittent failure in TestConfirmationsRemoveEvent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
time="2022-04-25T13:56:09-04:00" level=info msg="Added pending event TX:0x531e219d98d81dc9f9a14811ac537479f5d77a74bdba47629bfbebe2d7663ce7|BLOCK:/0x0e32d749a86cfaf551d528b5b121cea456f980a39e5b8136eb8e85dbc744a542|INDEX:|LOG:" job=blockConfirmationManager
time="2022-04-25T13:56:09-04:00" level=info msg="Created block filter: 0x7b9" job=blockConfirmationManager
time="2022-04-25T13:56:09-04:00" level=info msg="Block 1002 unavailable walking chain event=TX:0x531e219d98d81dc9f9a14811ac537479f5d77a74bdba47629bfbebe2d7663ce7|BLOCK:/0x0e32d749a86cfaf551d528b5b121cea456f980a39e5b8136eb8e85dbc744a542|INDEX:|LOG:" job=blockConfirmationManager
time="2022-04-25T13:56:09-04:00" level=debug msg="Block confirmation listener stopping" job=blockConfirmationManager
--- FAIL: TestConfirmationsRemoveEvent (0.00s)
    block_confirmations_test.go:616: 
        	Error Trace:	block_confirmations_test.go:616
        	Error:      	Should be empty, but was map[TX:0x531e219d98d81dc9f9a14811ac537479f5d77a74bdba47629bfbebe2d7663ce7|BLOCK:/0x0e32d749a86cfaf551d528b5b121cea456f980a39e5b8136eb8e85dbc744a542|INDEX:|LOG::0x1400038c1e0]
        	Test:       	TestConfirmationsRemoveEvent
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 18:13:07 +0000 UTC
    </div>
</div>

