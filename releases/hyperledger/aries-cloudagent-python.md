---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    1.0.0-rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.0.0-rc2
                </span>
            </td>
            <td>
                ACA-Py 1.0.0 will be a breaking update to ACA-Py with the version number indicating the maturity of the implementation. The final 1.0.0 release will be Aries Interop Profile 2.0-complete, and based on Python 3.9 or higher. The decision to start tagging early `1.0.0` releases was probably a bad one given the subsequent focus in the community on optimization of what we have vs. completing the [to-do list for AIP 2.0](/SupportedRFCs.md#aip-20). However, some organizations are using 1.0.0-rc1, so with this release of 1.0.0-rc2, we are providing an update that incorporates the many, many enhancements, improvements, and fixes that are in releases [0.8.0](#080) and [0.8.1](#081).

### Breaking Changes

See the breaking changes documented in Releases [0.8.1](#081) and [0.8.0](#080). There are no breaking changes in the merged pull requests listed below--those merged since Release 0.8.1.

## What's Changed

* fix: run only on main, forks ok by @anwalker293 in https://github.com/hyperledger/aries-cloudagent-python/pull/2166
* Add support for JsonWebKey2020 for the connection invitations by @dkulic in https://github.com/hyperledger/aries-cloudagent-python/pull/2173
* Update Alice Wants a JSON-LD Credential to fix invocation by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2219
* Disable webhook trigger on initial response to multi-use connection invitation by @esune in https://github.com/hyperledger/aries-cloudagent-python/pull/2223
* Fix broken link in README by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2221
* Fix formatting and grammatical errors in different readme's by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2222
* Connection target should not be limited only to indy dids by @dkulic in https://github.com/hyperledger/aries-cloudagent-python/pull/2229
* Multi-tenant self-managed mediation verkey lookup by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2232
* stand up multiple agents (single and multi) for local development and testing by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2230
* Fix multitenant/mediation in demo by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2075
* Upgrade codegen tools in `scripts/generate-open-api-spec` and publish Swagger 2.0 and OpenAPI 3.0 specs by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2246
* fix: route multitenant connectionless oob invitation by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/2243
* Add updated ELK stack for demos. by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2236
* ./run_demo performance -c 1 --mediation --timing --trace-log by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2245
* Bump requests from 2.30.0 to 2.31.0 in /demo/playground/scripts by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2238
* Pass document loader to jsonld.expand by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2175
* fix: only cache completed connection targets by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2240
* 1.0.0-rc2 Updates by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2253

## New Contributors
* @anwalker293 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2166
* @dkulic made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2173
* @ff137 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2221
* @usingtechnology made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2232
* @dependabot made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2238

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.8.1...1.0.0-rc2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/1.0.0-rc2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-05 15:48:13 +0000 UTC
    </span>
</div>

