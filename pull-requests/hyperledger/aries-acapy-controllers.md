---
layout: default
title: aries-acapy-controllers
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-controllers
---

# aries-acapy-controllers <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-controllers){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Centralize docker host IP script.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - This is an update to the previous commit to update the support for Docker networking.  The `getDockerHost` has been pulled out and placed in a central location where it can be updated as needed rather than having to update dozens of scripts the next time there is a change.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-08 21:04:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    Add support for changes to internal Docker networking.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Networking changes introduced in Docker 4.1.x and forward on Windows and MAC stop the direct use of the internal docker host IP returned by the `docker run --rm --net=host eclipse/che-ip` process. On Windows and MAC `host.docker.internal` needs to be used for internal connections between containers on separate docker networks.
- `host.docker.internal` has been available on Windows and Mac since Docker Engine version 18.03 (March 2018). Support for `host.docker.internal` on Linux was introduced in version 20.10.0 (2020-12-08), but it does not run out of the box yet (as of Docker Engine 20.10.11 (2021-11-17)). You need to add `--add-host=host.docker.internal:host-gateway` to the `docker run` command in order for it to work.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 20:48:03 +0000 UTC
    </div>
</div>

