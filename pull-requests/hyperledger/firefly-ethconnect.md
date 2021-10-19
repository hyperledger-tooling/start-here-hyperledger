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
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/169" class=".btn">#169</a>
            </td>
            <td>
                <b>
                    Fix push of latest docker tag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since this is the last line in the action, this is probably the last fix that will be needed :disappointed: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 11:48:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-ethconnect/pull/168" class=".btn">#168</a>
            </td>
            <td>
                <b>
                    Fix tagging of latest image on release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix the current problem with tagging latest on a release build
```
Run docker tag ghcr.io/hyperledger/firefly-ethconnect:latest ghcr.io/hyperledger/firefly-ethconnect:latest
  docker tag ghcr.io/hyperledger/firefly-ethconnect:latest ghcr.io/hyperledger/firefly-ethconnect:latest
  shell: /usr/bin/bash -e {0}
Error response from daemon: No such image: ghcr.io/hyperledger/firefly-ethconnect:latest
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 20:21:47 +0000 UTC
    </div>
</div>

