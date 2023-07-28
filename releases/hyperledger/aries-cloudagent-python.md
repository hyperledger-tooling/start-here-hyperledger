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
                    0.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.9.0
                </span>
            </td>
            <td>
                Release 0.9.0 is an important upgrade that changes (PR [\#2302]) the dependency on the now archived Hyperledger Ursa project to its updated, improved replacement, [AnonCreds CL-Signatures]. This important change is ONLY available when using [Aries Askar] as the wallet type, which brings in both [Indy VDR] and the CL-Signatures via the latest version of [CredX from the indy-shared-rs repository]. The update is **NOT** available to those that are using the [Indy SDK], which will continue to use the old Ursa implementation. All new deployments of ACA-Py SHOULD use [Aries Askar]. Further, we **strongly** recommend that all deployments using the [Indy SDK] with ACA-Py upgrade their installation to use [Aries Askar] and the related components using the migration scripts available. An [Indy SDK to Askar migration document] added to the [aca-py.org] documentation site, and a deprecation warning added to the ACA-Py startup.

[AnonCreds CL-Signatures]: https://github.com/hyperledger/anoncreds-rs
[Aries Askar]: https://github.com/hyperledger/aries-askar
[CredX from the indy-shared-rs repository]: https://github.com/hyperledger/indy-shared-rs
[Indy SDK]: https://github.com/hyperledger/indy-sdk
[Indy SDK to Askar migration document]: https://aca-py.org/main/deploying/IndySDKtoAskarMigration/
[aca-py.org]: https://aca-py.org

The second big change in this release is that we have upgraded the primary Python version from 3.6 to 3.9 (PR [\#2247]). In this case, primary means that Python 3.9 is used to run the unit and integration tests on all Pull Requests. We also do nightly runs of the main branch using Python 3.10. As of this release we have **dropped** Python 3.6, 3.7 and 3.8, and introduced new dependencies that are not supported in those versions of Python. For those that use the published ACA-Py container images, the upgrade should be easily handled. If you are pulling ACA-Py into your own image, or a non-containerized environment, this is a breaking change that you will need to address.

Please see the next section for all breaking changes, and the subsequent section for a categorized list of all pull requests in this release.

## Breaking Changes

In addition to the breaking Python 3.6 to 3.9 upgrade, there are two other breaking changes that may impact some deployments.

[\#2034] allows for additional flexibility in using public DIDs in invitations, and adds a restriction that "implicit" invitations must be proactively enabled using a flag (`--requests-through-public-did`). Previously, such requests would always be accepted if `--auto-accept` was enabled, which could lead to unexpected connections being established.

[\#2170] is a change to improve message handling in the face of delivery errors when using a persistent queue implementation such as the [ACA-Py Redis Plugin]. If you are using the Redis plugin, you **MUST** upgrade to [Redis Plugin Release 0.1.0] in conjunction with deploying this ACA-Py release. For those using their own persistent queue solution, see the PR [\#2170] comments for information about changes you might need to make to your deployment.

[ACA-Py Redis Plugin]: https://github.com/bcgov/aries-acapy-plugin-redis-events
[Redis Plugin Release 0.1.0]: https://github.com/bcgov/aries-acapy-plugin-redis-events/releases/tag/v0.1.0

[\#2302]: https://github.com/hyperledger/aries-cloudagent-python/pull/2302
[\#2034]: https://github.com/hyperledger/aries-cloudagent-python/pull/2034
[\#2247]: https://github.com/hyperledger/aries-cloudagent-python/pull/2247
[\#2170]: https://github.com/hyperledger/aries-cloudagent-python/pull/2170

## What's Changed
* Correct Daniel Hardman's github id by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/2286
* Add replacement_id to API. by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2273
* Minor revisions to the README.md and DevReadMe.md by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2272
* Add devcontainer for ACA-Py by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2267
* chore!: drop python 3.6 support by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2247
* BREAKING: feat: get queued outbound message in transport handle message by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2170
* Webhook over websocket clarification by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2287
* Fix routing in set public did by @mkempa in https://github.com/hyperledger/aries-cloudagent-python/pull/2288
* Add Explicit/Offline marking mechanism for Upgrade by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2204
* fix: use python 3.9 in run_docker by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2291
* Add Goal and Goal Code to OOB and DIDex Request by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2294
* Add build step for indy-base image in run_demo by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2299
* Cancel in-progress workflows when PR is updated by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2303
* Feature: JWT Sign and Verify Admin Endpoints with DID Support by @burdettadam in https://github.com/hyperledger/aries-cloudagent-python/pull/2300
* Fix alice/faber demo execution by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2305
* Feat: Added support for Ed25519Signature2020 signature type and Ed25519VerificationKey2020 by @dkulic in https://github.com/hyperledger/aries-cloudagent-python/pull/2241
* Add .indy_client folder to Askar only image. by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2308
* Allow any did to be public by @mkempa in https://github.com/hyperledger/aries-cloudagent-python/pull/2295
* Update to indy-credx 1.0 by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2302
* API endpoint to decommission revocation registry by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2309
* ⬆️ upgrade `marshmallow` to latest by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2322
* chore(deps): Bump aiohttp from 3.8.4 to 3.8.5 in /demo/playground/scripts by @dependabot in https://github.com/hyperledger/aries-cloudagent-python/pull/2325
* Added base wallet provisioning details to Multitenancy.md by @esune in https://github.com/hyperledger/aries-cloudagent-python/pull/2328
* chore: update PyYAML by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2329
* Fix: Track endorser and author roles in per-tenant settings by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2331
* Add revocation registry rotate to faber demo by @usingtechnology in https://github.com/hyperledger/aries-cloudagent-python/pull/2333
* ⬆️ upgrade `packaging` to latest by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2334
* ⬆️ upgrade `requests` to latest by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2336
* chore: add indy deprecation warnings by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2332
* 0.9.0-rc0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2338
* Document the Indy SDK to Askar Migration process by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2340
* Add more context to the ACA-Py Revocation handling documentation by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2343
* ⬆️ upgrade `pyjwt` to latest; introduce leeway to `jwt.decode` by @ff137 in https://github.com/hyperledger/aries-cloudagent-python/pull/2335
* 0.9.0 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2344


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.8.2...0.9.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.9.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-07-24 22:26:07 +0000 UTC
    </span>
</div>

