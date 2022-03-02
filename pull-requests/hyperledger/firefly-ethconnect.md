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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    Remove newline between fields in log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR removes a newline in a log that outputs the request ID and offset. Logging on the same line makes it easier to search for an offset or a request ID in the logs to correlate the lifecycle of a request (when received, when received on the consumer side, final response sent etc.)

So, instead of:

```
[2022-02-28T16:36:57.787Z]  INFO <-- POST /gateways/simplestorage [202]:
{"sent":true,"id":"942308fe-2fc9-435c-6690-6d249c563fb2","msg":"zzaaaaaaa-zzbbbbbbb-requests:0:71338"}
```

we will log:

```
[2022-02-28T16:36:57.787Z]  INFO <-- POST /gateways/simplestorage [202]: {"sent":true,"id":"942308fe-2fc9-435c-6690-6d249c563fb2","msg":"zzaaaaaaa-zzbbbbbbb-requests:0:71338"}
```

Signed-off-by: Vinod Damle <vinod.damle@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 19:21:55 +0000 UTC
    </div>
</div>

