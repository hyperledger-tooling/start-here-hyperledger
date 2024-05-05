---
layout: default
title: fabric-ansible-collection
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-ansible-collection
---

# fabric-ansible-collection <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-ansible-collection){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Correct the docker-entrypoint.sh to use hlf-user
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the docker-entrypoint.sh to use hlf-user instead of ibp-user

```
if ! whoami &> /dev/null; then
    sed '/hlf-user/d' /etc/passwd > /tmp/passwd
    cat /tmp/passwd > /etc/passwd
    rm -f /tmp/passwd
    echo "hlf-user:x:$(id -u):0::/home/hlf-user:/bin/bash" >> /etc/passwd
    export HOME=/home/hlf-user
fi
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 14:39:57 +0000 UTC
    </div>
</div>

