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

