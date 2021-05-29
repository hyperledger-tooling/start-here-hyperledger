---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    Refactor test harness to integrate auxiliary services, and add a local uniresolver service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Von-network and indy-tails-server are now 'services' that are automatically
started by the ./manage script when it runs tests. Additional services can
be added just like these, by creating a folder for the service inside
`services`, and creating a wrapper script in the style of the existing ones.

Adds a universal-resolver service with a sov driver, for agents to be able to
resolve published did:sov DIDs from the local VON network.

Adds agent-type-specific environment configuration, using an <agent-name>.env
file in the agent's folder.

Configures afgo-interop to use the local uniresolver for did:sov.

Refactors ./manage script to add new commands:
- service: subcommands to `start`/`stop` a service, view `logs`, delete&`clean`
- start: start services and agents
- test: execute tests on running agents
- stop: stop agents (but leaves services running, for faster subsequent tests)

`./manage run [agents] [other args]` is the same as:

    ./manage start [agents]
    ./manage run [other args]
    ./manage stop

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-26 18:19:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    WIP: aries-vcx backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-25 20:33:38 +0000 UTC
    </div>
</div>

