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
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/110" class=".btn">#110</a>
            </td>
            <td>
                <b>
                    Fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for running FireFly networks with Fabric on a local dev machine.

https://github.com/hyperledger/firefly/pull/184 is a prerequisite for this code to work, but not a prerequisite for merging, as merging this should not break any existing functionality.

To create a FireFly stack with fabric as the blockchain simply run:

```
ff init -b fabric
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 16:58:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Update registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the CLI to use the new registration endpoints (and stop using the deprecated endpoints) with `confirm=true`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 19:39:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-cli/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Fixes for docker-compose 2.0 compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses several issues:

- Fixes https://github.com/hyperledger/firefly-cli/issues/100
- Fixes https://github.com/hyperledger/firefly-cli/issues/106

The docker compose file now explicitly gives each container a name, rather than letting docker-compose name each container. This ensures that the naming is consistent across each version of docker-compose.

There is also extra code added to explicitly remove every volume created by the stack when `reset` is called, rather than depending on docker-compose to do that for us.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 19:17:29 +0000 UTC
    </div>
</div>

