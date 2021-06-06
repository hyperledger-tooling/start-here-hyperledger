---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    change docker-compose version from 2 to 2.4  on folder addOrg3/docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the instructions to set an organization 3, the docker-compose file (test-network/addOrg3/docker/docker-compose-org3.yaml) was invalid because it didn't accept additional properties in the network declaration (test_network) with docker-compose version 2. I was able to solve the problem by setting the version to 2.4.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-05 23:24:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/447" class=".btn">#447</a>
            </td>
            <td>
                <b>
                    Support docker.sock in rootless mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Docker version 20.10 support rootless mode. That features
changes a mount path of docker.sock.
This PR loads a mount path from DOCKER_HOST environment,
and if not set, a mount path will be /var/run/docker.sock

FAB-18481

Signed-off-by: Nao Nishijima <nao.nishijima.xt@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 09:36:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/446" class=".btn">#446</a>
            </td>
            <td>
                <b>
                    [FAB-18460] Broken link in Developing Applications Application
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add organization connection profiles that were deleted by mistake during a merge: [Update Commercial Paper to v2.0 Lifecycle](https://github.com/hyperledger/fabric-samples/commit/b89ee34ff745b76922f00049df07629baaf3fe5d).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 06:34:59 +0000 UTC
    </div>
</div>

