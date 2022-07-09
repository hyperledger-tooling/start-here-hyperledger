---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    Auth plugin framework
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the auth plugin framework and a simple basic auth plugin to the common library which can be used by each FireFly microservice. In the common library, it is applied at the HTTP listener level. However, other services can use the Authorize function however they need. For example, FireFly Core will also use the same function at a namespace level on HTTP requests, and WebSocket messages.

The basic auth plugin expects a `passwordfile` config key to be set, which should point to a file created with htpasswd using bcrypt hashed passwords. For example, you can create such a file by running:
```
htpasswd -cB allowed_users firefly
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 19:14:52 +0000 UTC
    </div>
</div>

