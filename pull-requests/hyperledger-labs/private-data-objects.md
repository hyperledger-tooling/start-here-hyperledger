---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/488" class=".btn">#488</a>
            </td>
            <td>
                <b>
                    Add comments to SW to address concerns in Issue 195
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adding comments to pdo tp and pservice code where enclave ias attesta…tion verification report is checked. Adding notes about the fact that currently we do not check whether the enclave runs in SGX debug mode or not. The corresponding issue can be found at https://github.com/hyperledger-labs/private-data-objects/issues/195
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-30 16:08:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/487" class=".btn">#487</a>
            </td>
            <td>
                <b>
                    Parameterize docker(-compose) commands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upstream docker doesn't work anymore with (ubuntu) docker-compose and relies now on a docker plugin (invoked as `docker compose`).  To enable both, parameterized invocation of docker-compose (and for consistency also docker) so upstream user can redefine `DOCKER_COMPOSE_COMMAND` to `docker compose` in `make.loc` 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 21:33:27 +0000 UTC
    </div>
</div>

