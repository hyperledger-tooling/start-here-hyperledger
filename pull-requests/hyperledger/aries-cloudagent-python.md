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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1900" class=".btn">#1900</a>
            </td>
            <td>
                <b>
                    feat: added message to forward event handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Strobel <peter@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 19:32:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1899" class=".btn">#1899</a>
            </td>
            <td>
                <b>
                    Feat/public did endpoints for agents behind mediators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR supports publishing endpoint information with routing keys in accordance with the did:sov specification. Routing keys are retrieved from `mediation_id` if specified, or else a default mediator. If no mediated connection is present, `routingKeys` defaults to an empty array. 

This PR allows for publishing DIDs with routing keys; PR #1863 allows for resolving DIDs with routing keys.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 23:23:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1897" class=".btn">#1897</a>
            </td>
            <td>
                <b>
                    Fixes a few AATH failures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes:
- one 023-did-exchange error
- 0434-oob errors
- one 0183-revocation error

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 18:46:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1896" class=".btn">#1896</a>
            </td>
            <td>
                <b>
                    [#1895] Stopping the aca-py shell process keeps python process running
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 09:16:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1894" class=".btn">#1894</a>
            </td>
            <td>
                <b>
                    Fix: SchemasInputDescriptorFilter: broken deserialization renders generated clients unusable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **What’s wrong?**
The OpenAPI spec requires an Input Descriptor’s `schema` property to contain a `SchemasInputDescriptorFilter` object.
However, on deserialization, there is a [preprocessing step](https://github.com/hyperledger/aries-cloudagent-python/blob/d407c48cc9f041c5b27ee8f589fc0e2eaef2220d/aries_cloudagent/protocols/present_proof/dif/pres_exch.py#L235-L254) which ensures that lists of URIs or a dict containing a `oneof_filter` property are accepted as well by transforming them into said object. (These alternative input formats are also [included as examples](https://github.com/hyperledger/aries-cloudagent-python/blob/d407c48cc9f041c5b27ee8f589fc0e2eaef2220d/aries_cloudagent/protocols/present_proof/dif/pres_exch.py#L640-L663) in the `InputDescriptors` model.) Yet, input that already IS a `SchemasInputDescriptorFilter` object is not handled correctly during preprocessing and deserialization fails. This results in any client adhering to the spec being unable to create valid input descriptors and, ultimately, a presentation definition to use in a DIF proof request.

**What has been changed?**
I adjusted the preprocessing step such that input is forwarded as-is if it looks like a `SchemasInputDescriptorFilter`. I also extended the tests to cover deserializing the actual object.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 15:58:06 +0000 UTC
    </div>
</div>

