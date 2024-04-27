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
                    0.12.1rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.12.1rc1
                </span>
            </td>
            <td>
                Release 0.12.1rc1 is a small patch to cleanup some edge case issues in the handling of Out of Band invitations, revocation notification webhooks, and connection querying uncovered after the 0.12.0 release. Fixes and improvements were also made to the generation of ACA-Py's OpenAPI specifications.

## 0.12.1rc1 Breaking Changes

There are no breaking changes in this release.

## What's Changed
* chore(deps): Bump idna from 3.6 to 3.7 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2887
* Some updates to the mkdocs publishing process by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2888
* Fix ack during for auto endorsement by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2883
* Prevent 500 error when re-promoting DID with endorsement by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2885
* fix: integration tests should use didex 1.1 by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2889
* fix: look up conn record by invite msg id instead of key by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2891
* :bug: Fix IndyAttrValue model that was dropped from openapi spec by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2894
* fix: oob record their_service should be updatable by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2897
* :arrow_up: Upgrade codegen tools used in generate-open-api-specols by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2899
* chore(deps): Bump psf/black from 24.3.0 to 24.4.0 in the all-actions group by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2893
* chore(deps): Bump idna from 3.4 to 3.7 in /demo/playground/examples by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2886
* fix: consider all resolvable dids in invites "public" by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2900
* :art: fix typos by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2898
* fix Faber demo to use oob with aip10 to support connection reuse by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2903
* chore(deps): Bump aiohttp from 3.9.3 to 3.9.4 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2902
* :bug: Fix ServiceDecorator parsing in oob record handling by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2910
* Fix api schema mixup in revocation routes by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2909
* refactor: logging configs setup by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/2870
* 0.12.1rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2912
* fix: rev notifications on publish pending by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2916
* Update AnonCreds to 0.2.2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2917
* fix: fixes a regression that requires a log file in multi-tenant mode by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/2918
* 0.12.1rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2921


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.12.0...0.12.1rc1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.12.1rc1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-04-26 23:23:55 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.12.1rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.12.1rc0
                </span>
            </td>
            <td>
                Release 0.12.1rc0 is a small patch to cleanup some edge case issues in the handling of Out of Band invitations and connection querying uncovered after the 0.12.0 release. Fixes and improvements were also made to the generation of ACA-Py's OpenAPI specifications.

### 0.12.1rc0 Breaking Changes

There are no breaking changes in this release.

## What's Changed
* chore(deps): Bump idna from 3.6 to 3.7 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2887
* Some updates to the mkdocs publishing process by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2888
* Fix ack during for auto endorsement by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2883
* Prevent 500 error when re-promoting DID with endorsement by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2885
* fix: integration tests should use didex 1.1 by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2889
* fix: look up conn record by invite msg id instead of key by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2891
* :bug: Fix IndyAttrValue model that was dropped from openapi spec by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2894
* fix: oob record their_service should be updatable by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2897
* :arrow_up: Upgrade codegen tools used in generate-open-api-specols by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2899
* chore(deps): Bump psf/black from 24.3.0 to 24.4.0 in the all-actions group by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2893
* chore(deps): Bump idna from 3.4 to 3.7 in /demo/playground/examples by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2886
* fix: consider all resolvable dids in invites "public" by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2900
* :art: fix typos by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2898
* fix Faber demo to use oob with aip10 to support connection reuse by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2903
* chore(deps): Bump aiohttp from 3.9.3 to 3.9.4 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2902
* :bug: Fix ServiceDecorator parsing in oob record handling by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2910
* Fix api schema mixup in revocation routes by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2909
* refactor: logging configs setup by @amanji in https://github.com/hyperledger/aries-cloudagent-python/pull/2870
* 0.12.1rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2912


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.12.0...0.12.1rc0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.12.1rc0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-04-24 19:52:49 +0000 UTC
    </span>
</div>

