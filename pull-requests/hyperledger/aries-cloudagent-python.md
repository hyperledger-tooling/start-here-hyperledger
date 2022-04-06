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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1714" class=".btn">#1714</a>
            </td>
            <td>
                <b>
                    Update raise errors and add schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: DaevMithran <daevmithran1999@gmail.com>

Updated pull request changes suggested by @TimoGlastra 

- Raising an http bad request error when a seed is passed in the body and wallet-allow-insecure-seed is not enabled
- Updated schema for wallet/did/create
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 11:38:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1711" class=".btn">#1711</a>
            </td>
            <td>
                <b>
                    Fixes for v7.3.0 - Issue#1597
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1597 
- Moved changes from PR #1610 to overcome the DCO issue from partially verified commit and subsequent manual sign-off. 
- More details and comments can be found [here](https://github.com/hyperledger/aries-cloudagent-python/pull/1610)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 18:12:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1710" class=".btn">#1710</a>
            </td>
            <td>
                <b>
                    feat: support connectionless exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for connectionnless exchange using ICv1, ICv2, PPv1 and PPv2 protocols for both roles (so issuer, holder and verifier).

Can be initiated by creating or receiving an oob invitation without handshake protocols. If a connection already exists for the did in the oob invitation service, the connection will be used instead (as specified in OOB RFC).

Fixes #1636

Some notes on the implementation:
- Added an `OobRecord` to keep track of the oob state. This is used for both connectionfull and connectionless exchanges and will be removed once the interaction is done
- The oob record will also emit events at the moment about reuse of connections etc... To not make breaking changes I kept the old OOB reuse webhook events in place. May be good to remove these in a future PR
- Connectionless is not integrated with mediation yet (when creating an invitation). If this is desired, maybe someone else can take a look at this
- I disabled multi use when attachments were present in the invitation as this would never have worked (there's no support for multi-use requests, offers AFAIK?)
- Adds a cleanup of stale connections if a connection is being reused by sending a direct response to an attachment message in the oob invitation (I think connections weren't being cleaned up in this case)

Keeping it in draft until I know for sure all CI tests have passed (can't run all tests on my M1 mac)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-05 13:36:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1709" class=".btn">#1709</a>
            </td>
            <td>
                <b>
                    run_docker start - specify argument from environment variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
- resolve #1330 
- @MonolithicMonk I think you are starting ACA-Py agent from `./scripts/run_docker start ...`. You can either specify the environment variables in `./scripts/run_docker` by adding each one of them as something like:
```
$CONTAINER_RUNTIME run --rm -ti --name "aries-cloudagent-runner_${RAND_NAME}" \
-e ACAPY_OUTBOUND_TRANSPORT=http -e ACAPY_INBOUND_TRANSPORT=[[\"http\",\"0.0.0.0\",\"8021\"],[\"ws\",\"0.0.0.0\",\"8023\"]] \
    $ARGS aries-cloudagent-run "$@"
```
- Another option [if this PR is approved and merged], is just to export the `environment variable` as usual. Updated script will go through all the `environment variables`, extract all with `*ACAPY_*` and `*=*` pattern match and add them to `docker run ... -e env_var -e env_var .....`.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 19:48:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1706" class=".btn">#1706</a>
            </td>
            <td>
                <b>
                    Multitenancy Docs Update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Please review the updates to the multitenancy docs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 17:01:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1705" class=".btn">#1705</a>
            </td>
            <td>
                <b>
                    Fix Issue-1682
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Added wallet startup parameter: --wallet-allow-insecure-seed
- support seed in wallet/did/create route

Some questions around
1. How do we support importing a key pair into the wallet as mentioned in the Issue
2. Should I add seed in the schema of wallet/did/create ? . I don't think we can add conditional schemas according to startup parameter.  I can have it as an optional field.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 10:56:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1702" class=".btn">#1702</a>
            </td>
            <td>
                <b>
                    Add auto_verify flag in present-proof protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: DaevMithran <daevmithran1999@gmail.com>

Fix [https://github.com/hyperledger/aries-cloudagent-python/issues/1698](url)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 12:57:29 +0000 UTC
    </div>
</div>

