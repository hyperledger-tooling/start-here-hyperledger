---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2095" class=".btn">#2095</a>
            </td>
            <td>
                <b>
                    feat: universal resolver - configurable authentication
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Context: we want to allow aca-py instances to connect to privately run universal resolvers such as the one from godiddy. This requires authentication.

* Add `--universal-resolver-bearer-token` to allow authentication against privately run universal resolvers.

BREAKING CHANGE:
Configured url should now include the `/1.0` suffix. The default url reflects that changes.
* This is to have a more flexible configuration of the universal resolver's api route (required in the case of godiddy).
* The alternative would be to make the suffix configurable too. I just found it a bit fiddly both in code and configuration. Let me know if the breaking change in configuration is not acceptable.

Signed-off-by: Clément Humbert <clement.humbert@sicpa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 10:49:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2094" class=".btn">#2094</a>
            </td>
            <td>
                <b>
                    Webhook Security
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: ram.challa <ram.challa@ontario.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-26 06:11:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2091" class=".btn">#2091</a>
            </td>
            <td>
                <b>
                    Allow using YAML configuration file with run_docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will allow using scripts like this:

```bash
#!/usr/bin/env bash

# Uncomment for debugging
# set -o xtrace

set -eo pipefail  # Exit the script if any statement returns error.

SCRIPT_DIR="$( dirname "$(readlink -f "$0")" )"

export CONTAINER_NAME="aries_issuer"
export NETWORK_NAME="aries-mediator-service_mediator-network"
export PORTS="8002 11002"
export ARG_FILE="${SCRIPT_DIR}/cfg_issuer.yml"

../aries-cloudagent-python/scripts/run_docker start
```

I find working with yaml files easier/faster than very, very long command line when testing and debugging (because I can simply comment out some configs and uncomment others at the same time).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-25 15:26:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2089" class=".btn">#2089</a>
            </td>
            <td>
                <b>
                    Multitenancy demo (docker-compose with postgres and ngrok)
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
        Created At 2023-01-24 17:28:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2088" class=".btn">#2088</a>
            </td>
            <td>
                <b>
                    Feat: Multiple Credential Issuance [v2.1]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>

- WIP
- resolves #1979
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-24 17:13:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2086" class=".btn">#2086</a>
            </td>
            <td>
                <b>
                    fix: create local DID return schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a follow-up to the changes in the creation endpoint (#2067), relax return schema to include any did method.

Without this change, clients based on the openapi spec cannot accept the response payload for did methods other than "sov" and "key".

Signed-off-by: Clément Humbert <clement.humbert@sicpa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-24 08:19:22 +0000 UTC
    </div>
</div>

