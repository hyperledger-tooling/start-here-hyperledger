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
                    0.11.0-rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.11.0-rc1
                </span>
            </td>
            <td>
                Release 0.11.0 is a relatively large release of new features, fixes, and internal updates. 0.11.0 is planned to be the last major update before we transition to using the [AnonCreds Rust](https://github.com/hyperledger/anoncreds-rs) in a release that is expected to bring some Admin/Controller API changes. We plan to do patches to 0.11.0 while the transition is made to the next breaking release.

*Release 0.11.0-rc0 failed to publish because of a reference to a dependency via its GitHub repository rather than to its published artifact.*

A significant addition to ACA-Py is support for signing and verifying [SD-JWT] verifiable credentials. We expect this to be the first of the changes to extend ACA-Py to support [OpenID4VC protocols].

[SD-JWT]: https://sdjwt.info/
[OpenID4VC protocols]: https://openid.net/wg/digital-credentials-protocols/

In the CI/CD realm, substantial changes were applied to the source base in switching from:

- `pip` to [Poetry](https://python-poetry.org/) for packaging and dependency management,
- Flake8 to [Ruff](https://docs.astral.sh/ruff/) for linting,
- `asynctest` to `IsolatedAsyncioTestCase` and `AsyncMock` objects now included in Python's builtin `unittest` package for unit testing.

These are necessary and important modernization changes, with the latter two triggering many (largely mechanical) changes to the codebase.

**NOTE:** In addition to these PRs in the 0-11.0-rc0 release, we also expect to include at least those [ACA-Py PRs labelled "0.11.0"] in the release.

[ACA-Py PRs labelled "0.11.0"]: https://github.com/hyperledger/aries-cloudagent-python/pulls?q=is%3Apr+label%3A0.11.0

### 0.11.0 Breaking Changes

In addition to the impacts of the change for developers in switching from `pip` to Poetry, the only significant breaking change is the (overdue) transition of ACA-Py to always use the new DIDComm message type prefix, changing the DID Message prefix from the old hardcoded `did:sov:BzCbsNYhMrjHiqZDTUASHg;spec` to the new hardcoded `https://didcomm.org` value, and using the new DIDComm MIME type in place of the old. The vast majority (all?) Aries deployments have long since been updated to accept both values, so this change just forces the use of the newer value in sending messages. In updating this, we retained the old configuration parameters most deployments were using (`--emit-new-didcomm-prefix` and `--emit-new-didcomm-mime-type`) but updated the code to set the configuration parameters to `true` even if the parameters were not set. See [PR \#2517].

[PR \#2517]: https://github.com/hyperledger/aries-cloudagent-python/pull/2517

## What's Changed
* #2289 Migrate to Poetry by @Gavinok in https://github.com/hyperledger/aries-cloudagent-python/pull/2436
* Swap out flake8 in favor of Ruff by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2438
* Update Python image version to 3.9.18 by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2456
* chore: add black back in as a dev dep by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2465
* feat: add timeout to did resolver resolve method by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2464
* Remove old routing protocol code by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2466
* fix: issue #2434: Change DIDExchange States to Match rfc160 by @anwalker293 in https://github.com/hyperledger/aries-cloudagent-python/pull/2461
* fix: version should be set by pyproject.toml by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2471
* fix: unique ids for services in legacy peer by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2476
* peer did 2/3 resolution by @Jsyro in https://github.com/hyperledger/aries-cloudagent-python/pull/2472
* Bugfix: Issue with write ledger pool when performing Accumulator sync by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2480
* Update steps for Manually Creating Revocation Registries by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2491
* Issue #2419 InvalidClientTaaAcceptanceError time too precise error if container timezone is not UTC by @Ennovate-com in https://github.com/hyperledger/aries-cloudagent-python/pull/2420
* Update devcontainer to read version from aries-cloudagent package by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2483
* Issue #2488 KeyError raised when Subject ID is not a URI by @Ennovate-com in https://github.com/hyperledger/aries-cloudagent-python/pull/2490
* fix: run tests script copying local env by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2495
* Feat/sd jwt implementation by @cjhowland in https://github.com/hyperledger/aries-cloudagent-python/pull/2487
* Use correct rust log level in dockerfiles  by @loneil in https://github.com/hyperledger/aries-cloudagent-python/pull/2499
* Remove unused dependencies by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2510
* Feat: Upgrade from tags and fix issue with legacy IssuerRevRegRecords [<=`v0.5.2`] by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2486
* Change arg_parse to always set --emit-new-didcomm-prefix and --emit-new-didcomm-mime-type to true by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2517
* Fix: Problem Report Before Exchange Established by @Ennovate-com in https://github.com/hyperledger/aries-cloudagent-python/pull/2519
* refactor: drop mediator_terms and recipient_terms by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2515
* Avoid multiple open wallet connections by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2521
* chore(deps): Bump urllib3 from 2.0.5 to 2.0.6 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2525
* chore(deps): Bump urllib3 from 2.0.2 to 2.0.6 in /demo/playground/scripts by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2524
* chore: update pydid by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2527
* :art: clarify LedgerError message when TAA is required and not accepted by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2545
* fix: correct minor typos by @Ennovate-com in https://github.com/hyperledger/aries-cloudagent-python/pull/2544
* Update .readthedocs.yaml by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2547
* Update .readthedocs.yaml by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2548
* fix: routing behind mediator  by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2536
* Feat: Support subwallet upgradation using the Upgrade command by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2529
* chore(deps): Bump urllib3 from 2.0.6 to 2.0.7 by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2552
* fix: taa rough timestamp timezone from datetime by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2554
* refactor: replace multiformats library by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2559
* fix: mediation routing keys as did key by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2516
* chore(deps): Bump urllib3 from 2.0.6 to 2.0.7 in /demo/playground/scripts by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2551
* fix: clean up requests and invites by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2560
* Update demo/playground scripts by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2562
* refactor: use did-peer-2 instead of peerdid by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2561
* Issue 2555 playground scripts readme by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2563
* Playground needs optionally external network by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2564
* chore: dependency updates by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2565
* fix: drop asynctest by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2566
* 0.11.0-rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2575
* chore: point to official sd-jwt lib release by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2573
* 0.11.0-rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2576

## New Contributors
* @Ennovate-com made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2420

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.10.1...0.11.0-rc1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.11.0-rc1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-10-30 23:11:16 +0000 UTC
    </span>
</div>

