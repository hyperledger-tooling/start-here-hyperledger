---
layout: default
title: firefly-cli
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-cli
---

# firefly-cli <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-cli){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/289" class=".btn">#289</a>
            </td>
            <td>
                <b>
                    Limit upgrade command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The existing upgrade command is pretty limited in what it is able to do. It simply rewrites the stack.json and docker-compose file with newer image tags from a different version manifest. If there is any additional migration (such as config changes) required between versions it will not work.

As an example, when we moved all of the containers to run as a non-root user the FireFly CLI also had to be updated to put config files in a different location which a non-root user could read. This change was _backward_ compatible with older versions of FireFly, but older versions of the CLI would not be able to generate the proper config for _newer_ versions of FireFly. Thus, simply swapping the image tag would not work to move from 1.2.x -> 1.3.x because of permissions changes.

This PR sets some guardrails on the upgrade command to allow it to apply patch releases only (which should not contain these types of changes), and does not allow downgrades.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 19:29:25 +0000 UTC
    </div>
</div>

