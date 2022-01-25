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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    Fixing Graceful Shutdown for Container Image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed in a K8s environment when testing https://github.com/hyperledger/firefly-helm-charts/pull/12 that ethconnect was very slow to shut down. Likely bc its not receiving the sigterm: https://hynek.me/articles/docker-signals/

> If you run your application from a shell script the regular way, your shell spawns your application in a new process and you 
> won’t receive signals from Docker.
>
> What you need to do is to tell your shell to replace itself with your application. For that exact purpose, shells have the exec > command (the similarity to the exec form before is not an accident: exec syscall).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 06:32:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Including Latest CA Certs in Docker Image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When trying to have Ethconnect connect to a remote Geth node secured via HTTPS we noticed we were getting invalid cert errors:
```
x509: certificate signed by unknown authority
```

In the process of testing to confirm this fixes this issue.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-22 18:01:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Add query support to / POST payload (webhook)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the "webhook" post on `/` to accept a new message type of `Query` (in addition to existing `SendTransaction` and `DeployContract` payloads).

The `Query` payload:
- Extends `SendTransaction` accepting all the same fields
- Adds a `blockNumber` field that defaults to `latest` and supports the same strings as the existing query APIs

https://github.com/kaleido-io/firefly-ethconnect/blob/e726955992f768362e875388eacd0252d148cfc9/internal/messages/messages.go#L148-L152

Here's a super minimal example to call the `get` method of simple storage (noting I've trimmed down the method ABI to just what's needed - you could put the full JSON in there, with `inputs` and `stateMutability` etc. etc.):

```json
{
    "headers": {
        "type": "Query"
    },
    "to": "0x93A82a40d0297c126b0c6ee8334A8639233F8d39",
    "method":   {
        "name": "get",
        "outputs": [{
            "type": "uint256",
            "internalType": "uint256"
        }]
    },
    "params": []
}
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 04:55:17 +0000 UTC
    </div>
</div>

