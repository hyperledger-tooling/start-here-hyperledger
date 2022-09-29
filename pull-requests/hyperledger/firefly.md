---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1079" class=".btn">#1079</a>
            </td>
            <td>
                <b>
                    Fix Docker Release GitHub Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Apparently `docker buildx` flags `--load` and `--push` cannot be used at the same time currently. So this change switches `load` to happen when doing a normal, native architecture build. But allows for pushes when doing multiarch builds.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 18:11:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1078" class=".btn">#1078</a>
            </td>
            <td>
                <b>
                    Fix Docker Release GitHub Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-28 17:43:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1077" class=".btn">#1077</a>
            </td>
            <td>
                <b>
                    Update dependencies for v1.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 20:06:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1076" class=".btn">#1076</a>
            </td>
            <td>
                <b>
                    Fix the example ff deploy command to specify ethereum
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew Whitehead <matthew.whitehead@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-27 12:33:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1075" class=".btn">#1075</a>
            </td>
            <td>
                <b>
                    Issue 1056
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
        Created At 2022-09-26 16:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1074" class=".btn">#1074</a>
            </td>
            <td>
                <b>
                    V1.1.x/mainline fix: Allow update of node using parent org identity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See #1073 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 23:21:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1073" class=".btn">#1073</a>
            </td>
            <td>
                <b>
                    V1.0.x fix: Allow update of node using parent org identity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing patching Node identity for Cert cycling, I found that in v1.0 we were missing the API from the Swagger, but it did exist

`PATCH` `namespaces/{ns}/identities/{iid}`

However, attempt to run it for a node resulted in the following - due to a discrepancy between the checking for the author of the message between identity creation, and identity update:
`[2022-09-22T22:39:53.629Z]  WARN node_0: Invalid identity update message 2ac79c71-3983-45a4-8942-7f1bc124225b - wrong author: did:firefly:org/org_0 dbtx=reAmSQrS role=aggregator`

This PR is a V1.0 stream fix to correct this. A separate PR will be needed for the V1.1 stream - in #1074 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 23:02:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1072" class=".btn">#1072</a>
            </td>
            <td>
                <b>
                    Fix acknowledgement for webhooks in non-reply, non-fastack cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Raised from #1025 

- Adds better logging
- Ensures we do a `DeliveryResponse` in the case of a non-`reply`, non-`fastack` webhook subscription
- Disabled `fastack` when `reply` is configured, as the reply would not be sent otherwise
- (Re)instate the lost `events` section in the config docs
- Correct the docs to reflect that if you want to retry on non-`2xx` error codes, you need to set `events.webhooks.retry`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 18:18:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1071" class=".btn">#1071</a>
            </td>
            <td>
                <b>
                    Load output of docker buildx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 14:34:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1070" class=".btn">#1070</a>
            </td>
            <td>
                <b>
                    use `cm.namespace` when generating contract URL's 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ~~Fixes error where namespace was not set when resolving contract API on create. This resulted in contract listener url's being broken in the `POST` response.~~

When generating contract URL's, always use the `ContractManager` namespace.

closes #1067 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-22 13:46:26 +0000 UTC
    </div>
</div>

