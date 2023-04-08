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
                    0.8.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.8.1
                </span>
            </td>
            <td>
                Version 0.8.1 is an urgent update to Release 0.8.0 to address an inability to execute the `upgrade` command. The `upgrade` command is needed for 0.8.0 Pull Request [\#2116] - "UPGRADE: Fix multi-use invitation performance", which is useful for (at least) deployments of ACA-Py as a mediator. In the release, the upgrade process is revamped, and documented in [Upgrading ACA-Py].

Key points about upgrading for those with production, pre-0.8.1 ACA-Py deployments:

- Upgrades now happen **automatically** on startup, when needed.
- The version of the last executed upgrade, even if it is a "no change" upgrade, is put into secure storage and is used to detect when future upgrades are needed.
  - Upgrades are needed when the running version is greater than the version is secure storage.
- If you have an existing, pre-0.8.1 deployment with many connection records, there may be a delay in starting as an upgrade will be run that loads and saves every connection record, updating the data in the record in the process.
  - A mechanism is to be added (see [Issue #2201]) for preventing an upgrade running if it should not be run automatically, and requires using the `upgrade` command. To date, there has been no need for this feature.
- See the [Upgrading ACA-Py] document for more details.

### Postgres Support with Aries Askar

Recent changes to [Aries Askar] have resulted in Askar supporting Postgres version 11 and greater. If you are on Postgres 10 or earlier and want to upgrade to use Askar, you must migrate your database to Postgres 10.

We have also noted that in some container orchestration environments such as [Red Hat's OpenShift] and possibly other [Kubernetes] distributions, Askar using [Postgres] versions greater than 14 do not install correctly. Please monitor [Issue \#2199] for an update to this limitation. We have found that Postgres 15 does install correctly in other environments (such as in `docker compose` setups).

[\#2116]: https://github.com/hyperledger/aries-cloudagent-python/issues/2116
[Upgrading ACA-Py]: ./UpgradingACA-Py.md
[Issue #2201]: https://github.com/hyperledger/aries-cloudagent-python/issues/2201
[Aries Askar]: https://github.com/hyperledger/aries-askar
[Red Hat's OpenShift]: https://www.openshift.com/products/container-platform/
[Kubernetes]: https://kubernetes.io/
[Postgres]: https://www.postgresql.org/
[Issue \#2199]: https://github.com/hyperledger/aries-cloudagent-python/issues/2199

## What's Changed
* Adds the upgrade command YML file to the PyPi Release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2179
* Add link to recorded session about the ACA-Py Integration tests by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2184
* Update and automate ACA-Py upgrade process by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2185
* Create UnitTests.md by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2183
* 0.8.1-rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2190
* Fix: Resolve Upgrade Config file in Container by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2193
* 0.8.1-rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2194
* Fix: Indy WalletAlreadyOpenedError during upgrade process by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2196
* 0.8.1-rc2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2198
* Change upgrade definition file entry from 0.8.0 to 0.8.1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2203
* Doc update and some test scripts by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2189
* 3.7 and 3.10 unittests fix by @Jsyro in https://github.com/hyperledger/aries-cloudagent-python/pull/2187
* Add Upgrading ACA-Py document by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2200
* 0.8.1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2207

## New Contributors
* @Jsyro made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2187

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.8.0...0.8.1
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.8.1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-04-06 14:38:13 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.8.1-rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.8.1-rc2
                </span>
            </td>
            <td>
                An urgent update to Release 0.8.1 to address an inability to execute the upgrade command. The upgrade command is needed for Pull Request https://github.com/hyperledger/aries-cloudagent-python/pull/2116 - "UPGRADE: Fix multi-use invitation performance", which is necessary for (at least) deployments of ACA-Py as a mediator. The important updates are Pull Requests https://github.com/hyperledger/aries-cloudagent-python/pull/2185 and https://github.com/hyperledger/aries-cloudagent-python/pull/2196 (listed below). Documentation on upgrades in ACA-Py will be included before the final 0.8.1 release is tagged.

## What's Changed
* Adds the upgrade command YML file to the PyPi Release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2179
* Add link to recorded session about the ACA-Py Integration tests by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2184
* Update and automate ACA-Py upgrade process by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2185
* Create UnitTests.md by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2183
* 0.8.1-rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2190
* Fix: Resolve Upgrade Config file in Container by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2193
* 0.8.1-rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2194
* Fix: Indy WalletAlreadyOpenedError during upgrade process by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2196
* 0.8.1-rc2 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2198


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.8.0...0.8.1-rc2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.8.1-rc2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-04-04 13:43:54 +0000 UTC
    </span>
</div>

