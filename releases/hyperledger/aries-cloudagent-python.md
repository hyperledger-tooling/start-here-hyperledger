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
                    0.8.2-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.8.2-rc0
                </span>
            </td>
            <td>
                Release 0.8.2 contains a number of minor fixes and updates to ACA-Py, including the correction of a regression in Release 0.8.0 related to the use of plugins (see [\#2255]). Highlights include making it easier to use tracing in a development environment to collect detailed performance information about what is going in within ACA-Py.

There are no breaking changes in this release.

For more about this release, please see the [CHANGELOG.md](https://github.com/hyperledger/aries-cloudagent-python/blob/1.0.0-rc2/CHANGELOG.md) file.

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
* Resolve definitions.py fix by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2255
* Allow Log Access at Tenant Level by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2234
* Release 0.8.2-rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2260

## New Contributors
* @anwalker293 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2166
* @dkulic made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2173
* @ff137 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2221
* @usingtechnology made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2232
* @dependabot made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2238

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.8.1...0.8.2-rc0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.8.2-rc0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-06-08 21:32:30 +0000 UTC
    </span>
</div>

