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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    Inflight reset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently every time FireFly starts, it resets the EthConnect stream with a `PATCH` in order to apply any changes.
I observed a problem where a stream did not continue sending events after such an event.

I was able to produce a problem running two simple `curl` loops, where one stream stalled:

### 1. Sending messages with confirm

```sh
while [ 1 ]; do echo POSTING $(date); curl -s -X POST -d '{"data":[{"value":"test"}]}' -H "Content-type: application/json" 'localhost:5000/api/v1/namespaces/default/messages/broadcast?confirm' | jq; sleep 1; done
```

### 2. Resetting the stream

```sh
while [ 1 ]; do echo RESET $(date); curl -s -X PATCH -d @/tmp/ev.json  -H "Content-type: application/json" 0.0.0.0:5102/eventstreams/es-9f5df9e3-563e-4f11-7750-5d147ccf0231; sleep 1; done
```

There was not anything in the logs that really showed why the stream had stopped distributing data, and nothing in a `goroutine` dump. So I spent some time on code inspection, and made the changes in this PR.

- Reset the `InFlight` count to zero on update
    - This seemed to be a straight bug, and after fixing this I was not able to reproduce the stall
- Add better logging in case it happens again
    - Particularly per-polling loop debug when `InFlight > 0`
- Do not restart a stream if a `PATCH` does not result in any change
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 18:22:36 +0000 UTC
    </div>
</div>

