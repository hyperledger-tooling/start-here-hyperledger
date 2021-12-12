---
layout: default
title: aries-mediator-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mediator-service
---

# aries-mediator-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mediator-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/15" class=".btn">#15</a>
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
        Created At 2021-12-08 21:06:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/14" class=".btn">#14</a>
            </td>
            <td>
                <b>
                    Ssl
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
        Created At 2021-12-07 21:52:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/13" class=".btn">#13</a>
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
        Created At 2021-12-07 20:58:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/12" class=".btn">#12</a>
            </td>
            <td>
                <b>
                    Fix dependency versions (dependabot)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-07 20:31:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mediator-service/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Mediator refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Create manage script and refactor code into acapy sub-directory
Add optional demo controller; add support for play-with-docker

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-06 23:51:00 +0000 UTC
    </div>
</div>

