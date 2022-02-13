---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    Fix possibility for nil access in sendloop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for #485 with a bonus fix for this timing issue I'm seeing intermittently since upgrading my laptop.

```
time="2022-02-07T13:21:00-05:00" level=info msg="API server context cancelled - shutting down"
time="2022-02-07T13:21:00-05:00" level=info msg="API server complete"
--- FAIL: TestTLSServerSelfSignedWithClientAuth (0.13s)
    http_server_test.go:197: 
                Error Trace:    http_server_test.go:197
                Error:          Received unexpected error:
                                context deadline exceeded
                Test:           TestTLSServerSelfSignedWithClientAuth
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 19:03:54 +0000 UTC
    </div>
</div>

