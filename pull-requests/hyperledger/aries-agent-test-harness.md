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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    style: format with black
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Format all python files with black. Mostly to prevent a lot of formatting noise in upcoming PRs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 10:37:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 03:52:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/427" class=".btn">#427</a>
            </td>
            <td>
                <b>
                    feat: mediator coordination protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds initial support for the mediation coordination protocol. Had to change some things up as not all steps were set up to work with multiple connections being created in one test. Adds the endpoints to the OpenAPI spec.

I tried a new structure for backchannel topics in the AFGO / ACA-Py channel by giving the the topic it's own file and each route it's own method. the `xxx_backchannel` is getting quite complex making it hard to know what to change. What do you think of this approach? It's not all or nothing, so we can slowly adopt this mechanism for new topics. It's a similar pattern followed by the non python based backchannels.

This adds support for ACA-Py <-> ACA-Py and AFGO <-> AFGO mediation testing. Will add more interop testing between the two, and also support for agents without endpoint soon.

AFGO doesn't support mediate-deny so ignore the mediate deny test:

```
LEDGER_URL_CONFIG=http://test.bcovrin.vonx.io TAILS_SERVER_URL_CONFIG=https://tails.vonx.io ./manage run -d afgo-master -t @RFC0211 -t ~@T003-RFC0211
```

ACA-Py:

```
LEDGER_URL_CONFIG=http://test.bcovrin.vonx.io TAILS_SERVER_URL_CONFIG=https://tails.vonx.io ./manage run -d acapy-main -t @RFC0211
```

The mediator is just the agents that already existed. The frameworks all support being a mediator in addition to the other agent functionalities. We could decide to split it out to a different agent (Faythe) as described in #272.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 17:21:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/426" class=".btn">#426</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-03 03:52:27 +0000 UTC
    </div>
</div>

