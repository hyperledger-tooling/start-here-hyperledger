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
                    0.12.2rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.12.2rc1
                </span>
            </td>
            <td>
                A patch release to add the verification of a linkage between an inbound message and its associated connection (if any) before processing the message. Also adds some additional cleanup/fix PRs from the main branch (see list below) that might be useful for deployments currently using [Release 0.12.1](#0121).

## 0.12.2rc1 Breaking Changes

There are no breaking changes in this release.

## 0.12.2rc1 List of Pull Requests From The `main` Branch

- Check connection is ready in all connection required handlers [\#3095](https://github.com/hyperledger/aries-cloudagent-python/pull/3095) [jamshale](https://github.com/jamshale)
- fix: multiuse invites with did peer 4 [\#3112](https://github.com/hyperledger/aries-cloudagent-python/pull/3112) [dbluhm](https://github.com/dbluhm)
- fix: respond to did:peer:1 with did:peer:4 [\#3050](https://github.com/hyperledger/aries-cloudagent-python/pull/3050) [dbluhm](https://github.com/dbluhm)
- feat: soft binding for plugin flexibility [\#3010](https://github.com/hyperledger/aries-cloudagent-python/pull/3010) [dbluhm](https://github.com/dbluhm)
- feat: inject profile and session [\#2997](https://github.com/hyperledger/aries-cloudagent-python/pull/2997) [dbluhm](https://github.com/dbluhm)
- feat: external signature suite provider interface [\#2835](https://github.com/hyperledger/aries-cloudagent-python/pull/2835) [dbluhm](https://github.com/dbluhm)
- fix(interop): overly strict validation [\#2943](https://github.com/hyperledger/aries-cloudagent-python/pull/2943) [dbluhm](https://github.com/dbluhm)

## What's Changed
* Patch release 0.12.x by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3121
* 0.12.2rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/3123

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.12.1...0.12.2rc1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.12.2rc1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-25 16:21:17 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.11.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.11.2
                </span>
            </td>
            <td>
                A patch release to add the verification of a linkage between an inbound message and its associated connection (if any) before processing the message.

## 0.11.2 Breaking Changes

There are no breaking changes in this release.

## 0.11.2 List of Pull Requests from `main` Branch

- Check connection is ready in all connection required handlers [\#3095](https://github.com/hyperledger/aries-cloudagent-python/pull/3095) [jamshale](https://github.com/jamshale)

## What's Changed
* Apply security patch 0.11.x by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3120
* 0.11.2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/3122


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.11.1...0.11.2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.11.2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-25 16:20:56 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    1.0.0rc5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.0.0rc5
                </span>
            </td>
            <td>
                Release 1.0.0rc5 includes well over 100 PRs merged since [Release 0.12.1](#0121). The vast majority of that work was in hardening the product in preparation for this 1.0.0 release. While there are a number of new features, the majority of the focus has been on eliminating technical debt and improving the underlying implementation. The full list of PRs in this release can be [found below](#100rc5-categorized-list-of-pull-requests). here are the highlights of the release:

- The default underlying Python version has been upgraded to 3.12. Happily, there were minimal code changes to enable the upgrade to 3.12 from the previous Python 3.9.
- Pagination support has been added to a number of Admin API queries for object lists, enabling the development of better user interfaces for large deployments.
- Cleanup in the ACA-Py AnonCreds Revocation Registry handling to prevent errors that were found occurring under certain specific conditions.
- Upgraded pull request and release pipeline, including:
  - Enabling a much more aggressive approach to dependabot notifications, beyond just those for security vulnerabilities. Along with those upgrades, we've moved to newer/better build pipeline tooling, such as switching from Black to Ruff, and re-enable per pull request code coverage notifications.
    - Many of the PRs in this release are related to dependency updates from dependabot or applied directly.
  - A switch to more used tooling, such as a switch from black to ruff.
  - Improvements in coverage monitoring of pull requests.
- The start of a [DIDComm v2](https://identity.foundation/didcomm-messaging/spec/) implementation in ACA-Py. The work is not complete, as we are taking an incremental approach to adding DIDComm v2 support.
- A decorator has been added for enabling direct support for Admin API authentication. Previously, the only option to enable (the necessary) Admin API was to put the API behind a proxy that could manage authentication. With this update, ACA-Py deployments can handle authentication directly, without a proxy.
- We have dropped support for the old, archived [Indy SDK]. If you have not migrated your deployment off of the Indy SDK, you must do so now. See this [Indy SDK to Askar migration documentation](#https://aca-py.org/latest/deploying/IndySDKtoAskarMigration/) for guidance.
- Support added for using AnonCreds in [W3C VCDM](https://www.w3.org/TR/vc-data-model-1.1/) format.
 
### 1.0.0rc5 Breaking Changes

With the focus of the pull requests for this release on stabilizing the implementation, there were a few breaking changes:

- The default underlying Python version has been upgraded to 3.12.
- Support for the Indy SDK has been dropped. It had been previously deprecated. See this [Indy SDK to Askar migration documentation](#https://aca-py.org/latest/deploying/IndySDKtoAskarMigration/) for guidance.
- The webhook sent after receipt of presentation by a verifier has been updated to include all of the information needed by the verifier so that the controller does not have to call the "Verify Presentation" endpoint. The issue with calling that endpoint after the presentation has been received is that there is a race condition between the controller and the ACA-Py cleanup process deleting completed Present Proof protocol instances. See [\#3081](https://github.com/hyperledger/aries-cloudagent-python/pull/3081) for additional details.
- A fix to an obscure bug includes a change to the data sent to the controller after publishing multiple, endorsed credential definition revocation registries in a single call. The bug fix was to properly process the publishing. The breaking change is that when the process (now successfully) completes, the controller is sent the list of published credential definitions. Previously only a single value was being sent. See PR [\#3107](https://github.com/hyperledger/aries-cloudagent-python/pull/3107) for additional details.

## What's Changed
* Update README.md by @KPCOFGS in https://github.com/hyperledger/aries-cloudagent-python/pull/2927
* chore(deps): Bump ecdsa from 0.16.1 to 0.19.0 in the pip group across 1 directory by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2933
* feat: Integrate AnonCreds with W3C VCDI Format Support in ACA-Py by @sarthakvijayvergiya in https://github.com/hyperledger/aries-cloudagent-python/pull/2861
* Upgrade to anoncreds via api endpoint by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2922
* Feature: use decorators for admin api authentication by @esune in https://github.com/hyperledger/aries-cloudagent-python/pull/2860
* Anoncreds - Send full registry list when getting revocation states by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2946
* Example integration test issuing 2 credentials under the same schema by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2948
* Fix Snyk Container scanning workflow by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2951
* :arrow_up: Upgrade pydid (pydantic v2) by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2919
* Switch Snyk Container scan back to on push. by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2953
* Add OpenSSF Scorecard GHA - weekly by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2955
* :arrow_up: Upgrade test and lint dependencies by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2939
* feat: drop indy sdk by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2892
* fix(interop): overly strict validation by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2943
* Fix clear revocation logic by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2956
* Fix Snyk sarif file by @pradeepp88 in https://github.com/hyperledger/aries-cloudagent-python/pull/2961
* Add anoncreds migration guide by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2881
* chore: updating dependabot to support gha, python, docker and dev container packages by @rajpalc7 in https://github.com/hyperledger/aries-cloudagent-python/pull/2945
* Fix issue with requested to revoke before registry creation by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2995
* Sonarcloud with code coverage by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2968
* Manage integration tests with GitHub Actions (#2952) by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/2996
* :arrow_up: Upgrade `aiohttp-apispec` and `apispec` by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2920
* chore(deps): Bump untergeek/curator from 8.0.2 to 8.0.15 in /demo/elk-stack/extensions/curator by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2969
* feat: inject profile and session by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2997
* :sparkles: Faster uuid generation by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2994
* chore(deps): Bump sphinx-rtd-theme from 1.1.1 to 1.3.0 in /docs by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2970
* chore(deps): Bump hyperledger/aries-cloudagent-python from py3.9-0.9.0 to py3.9-0.12.1 in /demo/docker-agent by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2973
* chore(deps): Bump hyperledger/aries-cloudagent-python from py3.9-0.10.4 to py3.9-0.12.1 in /demo/playground by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2975
* Postgres Demo - Upgrade postgres and change entrypoint file by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3004
* chore(deps): Bump hyperledger/aries-cloudagent-python from py3.9-0.9.0 to py3.9-0.12.1 in /demo/multi-demo by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2976
* Merge all poetry dependabot PRs by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/3007
* Merge all demo dependabot PRs by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/3008
* Switch from pytz to dateutil by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3012
* Add sonarcloud badges by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3014
* chore(deps): Bump actions/checkout from 3 to 4 in the all-actions group by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3011
* feat: soft binding for plugin flexibility by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/3010
* Use a published version of aiohttp-apispec by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3019
* Add support for revocable credentials in vc_di handler by @EmadAnwer in https://github.com/hyperledger/aries-cloudagent-python/pull/2967
* chore(deps): Bump pydid from 0.5.0 to 0.5.1 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3024
* chore(deps-dev): Bump pytest from 8.2.1 to 8.2.2 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3025
* chore(deps): Update prompt-toolkit requirement from ~=2.0.9 to ~=2.0.10 in /demo by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3026
* chore(deps): Bump sphinx from 1.8.4 to 1.8.6 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3021
* docs: added section on environment variables by @Executioner1939 in https://github.com/hyperledger/aries-cloudagent-python/pull/3028
* :sparkles: Adds support for paginated storage queries, and implements pagination for the wallets_list endpoint by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/3000
* chore(deps): Bump dawidd6/action-download-artifact from 3 to 5 in the all-actions group by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3027
* chore(deps): Bump uuid-utils from 0.7.0 to 0.8.0 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3034
* chore(deps): Bump configargparse from 1.5.5 to 1.7 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3035
* chore(deps): Bump mkdocs-material from 9.5.10 to 9.5.27 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3036
* chore(deps): Bump packaging from 23.1 to 23.2 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3037
* chore(deps): Bump marshmallow from 3.20.2 to 3.21.3 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3038
* chore(deps): Bump urllib3 from 2.2.1 to 2.2.2 in /demo/playground/examples in the pip group by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3045
* Fix - only run integration tests on opened PR's by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3042
* Fix and refactor anoncreds revocation recovery by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3029
* Prevent getting stuck with no active registry by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3032
* chore(deps): Bump the pip group with 2 updates by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3046
* :adhesive_bandage: add exception handling to wallet-upgrade check by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/3048
* Handle failed tails server issuance [Anoncreds] by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3049
* fix: didexchange manager not checking the did-rotate content correctly by @gmulhearn-anonyome in https://github.com/hyperledger/aries-cloudagent-python/pull/3057
* Enable `no-transport` mode as startup parameter by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/2990
* chore(deps): Bump dawidd6/action-download-artifact from 5 to 6 in the all-actions group by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3064
* chore(deps): Bump markupsafe from 2.0.1 to 2.1.5 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3062
* :sparkles: Add pagination support for listing Connection, Cred Ex, and Pres Ex records by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/3033
* chore(deps-dev): Bump pydevd-pycharm from 193.6015.41 to 193.7288.30 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3060
* chore(deps-dev): Bump ruff from 0.4.4 to 0.4.10 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3058
* For proof problem handler, allow no connection record (OOB cases), prevent unhandled exception by @loneil in https://github.com/hyperledger/aries-cloudagent-python/pull/3068
* Re-enable ledger plugin when `--no-legder` is set by @PatStLouis in https://github.com/hyperledger/aries-cloudagent-python/pull/3070
* chore(deps): Bump requests from 2.32.2 to 2.32.3 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3076
* chore(deps): Bump uuid-utils from 0.8.0 to 0.9.0 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3075
* chore(deps-dev): Bump ruff from 0.4.10 to 0.5.0 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3073
* chore(deps): Bump mike from 2.0.0 to 2.1.2 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3074
* DIDComm V2 Initial Implementation by @TheTechmage in https://github.com/hyperledger/aries-cloudagent-python/pull/2959
* fix: respond to did:peer:1 with did:peer:4 by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/3050
* fix: print provision messages when auto-provision is triggered by @TheTechmage in https://github.com/hyperledger/aries-cloudagent-python/pull/3077
* Use anoncreds registry for holder credential endpoints by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3063
* Rule D417 by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3072
* Add by_format to terse webhook for presentations by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/3081
* :bug: fix storage record pagination with post-filter query params by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/3082
* Switch from black to ruff by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3080
* :art: improve record querying logic by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/3083
* Upgrade python to version 3.12 by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3067
* chore(deps): Bump certifi from 2024.6.2 to 2024.7.4 in the pip group by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3085
* :bug: fix IndyAttrValue bad reference in OpenAPI spec by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/3090
* chore(deps): Bump mkdocs-material from 9.5.27 to 9.5.28 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3089
* chore(deps-dev): Bump ruff from 0.5.0 to 0.5.1 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3087
* chore(deps): Bump aries-askar from 0.3.1 to 0.3.2 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3088
* chore(deps): Bump certifi from 2024.6.2 to 2024.7.4 in /demo/playground/examples in the pip group by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3084
* 1.0.0rc4 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/3092
* Update the docs for latest release and improve the publish flow and documentation by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/3097
* Add DIF presentation exchange context and cache document by @gmulhearn in https://github.com/hyperledger/aries-cloudagent-python/pull/3093
* VC DI proof request by @sarthakvijayvergiya in https://github.com/hyperledger/aries-cloudagent-python/pull/2960
* Library update 15/07/24 / Fix unit test typing by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3103
* Check connection is ready in all connection required handlers by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3095
* Fix the check for vc_di proof by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/3106
* Make single wallet config more explicit by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3105
* Breaking: Fix publishing multiple rev reg defs with endorsement by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3107
* Add descriptive error for issuance without RevRegRecord by @jamshale in https://github.com/hyperledger/aries-cloudagent-python/pull/3109
* chore(deps-dev): Bump pytest from 8.2.2 to 8.3.1 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3115
* chore(deps-dev): Bump pytest-ruff from 0.4.0 to 0.4.1 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3113
* chore(deps): Bump pytest-asyncio from 0.23.7 to 0.23.8 in /demo/playground/examples by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3117
* chore(deps-dev): Bump ruff from 0.5.2 to 0.5.4 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/3114
* fix: multiuse invites with did peer 4 by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/3112
* 1.0.0rc5 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/3118

## New Contributors
* @KPCOFGS made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2927
* @rajpalc7 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2945
* @EmadAnwer made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2967
* @Executioner1939 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/3028
* @gmulhearn made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/3093

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.12.1...1.0.0rc5
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/1.0.0rc5" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-07-23 19:11:27 +0000 UTC
    </span>
</div>

