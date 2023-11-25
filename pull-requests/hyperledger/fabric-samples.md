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
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1140" class=".btn">#1140</a>
            </td>
            <td>
                <b>
                    add support for docker compose v2 (fix #730)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Linux servers with docker engine installed through [docker document](https://docs.docker.com/engine/install/ubuntu/#install-using-the-repository) could not run `network.sh` successfully due to docker compose version compatibility. The default docker engine doesn't support `docker-compose` command.

As the [docker document](https://docs.docker.com/compose/migrate/#what-does-this-mean-for-my-projects-that-use-compose-v1) suggest, `docker compose` is preferred to use in docker compose V2.

This PR adds support for docker compose V2 version. It uses `docker compose` command if it finds `docker-compose` command fails to execute.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-25 12:45:41 +0000 UTC
    </div>
</div>

