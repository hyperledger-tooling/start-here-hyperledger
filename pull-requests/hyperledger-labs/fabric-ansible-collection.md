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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    Update ansible collection docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update base image to ubi9 minimal
- Upgrade golang to 1.21.9
- Upgrade Hyperledger Fabric to v2.5.7
- Add osnadmin binary
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-27 21:04:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Correct linter issues
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-27 18:57:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Add support for updating metadata for imported CAs, peer and ordering…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                … nodes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-26 13:08:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-ansible-collection/pull/57" class=".btn">#57</a>
            </td>
            <td>
                <b>
                    Add imported flag to CA, peer and ordering service node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 18:42:51 +0000 UTC
    </div>
</div>

