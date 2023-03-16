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
                    0.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.8.0
                </span>
            </td>
            <td>
                0.8.0 is a breaking change that contains all updates since release 0.7.5. It extends the previously tagged `1.0.0-rc1` release because it is not clear when the 1.0.0 release will be finalized. Many of the PRs in this release were previously included in the `1.0.0-rc1` release. The categorized list of PRs in the [CHANGELOG.md](https://github.com/hyperledger/aries-cloudagent-python/blob/0.8.0/CHANGELOG.md#080) separates those that are new from those in the `1.0.0-rc1` release candidate.

There are not a lot of new Aries Framework features in this release, as the focus has been on cleanup and optimization. The biggest addition is the inclusion with ACA-Py of a universal resolver interface, allowing an instance to have both local resolvers for some DID Methods and a call out to an external universal resolver for other DID Methods. Another significant new capability is full support for Hyperledger Indy transaction endorsement for Authors and Endorsers. A new repo [aries-endorser-service](https://github.com/hyperledger/aries-endorser-service) has been created that is a pre-configured instance of ACA-Py for use as an Endorser service.

A recently completed feature that is outside of ACA-Py is a script to migrate existing ACA-Py storage from Indy SDK format to Aries Askar format. This enables existing deployments to switch to using the newer Aries Askar components. For details see the converter in the [aries-acapy-tools](https://github.com/hyperledger/aries-acapy-tools) repository.

### Container Publishing Updated

With this release, a new automated process publishes container images in the Hyperledger container image repository. New images for the release are automatically published by the GitHubAction Workflows: [publish.yml] and [publish-indy.yml]. The actions are triggered when a release is tagged, so no manual action is needed. The images are published in the [Hyperledger Package Repository under aries-cloudagent-python] and a link to the packages added to the repositories main page (under "Packages"). Additional information about the container image publication process can be found in the document [Container Images and Github Actions].

The ACA-Py container images are based on [Python 3.6 and 3.9 `slim-bullseye` images](https://hub.docker.com/_/python), and are designed to support `linux/386 (x86)`, `linux/amd64 (x64)`, and `linux/arm64`. However, for this release, the publication of multi-architecture containers is disabled. We are working to enable that through the updating of some dependencies that lack that capability. There are two flavors of image built for each Python version. One contains only the Indy/Aries Shared Libraries only ([Aries Askar](https://github.com/hyperledger/aries-askar), [Indy VDR](https://github.com/hyperledger/indy-vdr) and [Indy Shared RS](https://github.com/hyperledger/indy-shared-rs), supporting only the use of`--wallet-type askar`). The other (labelled `indy`) contains the Indy/Aries shared libraries and the Indy SDK (considered deprecated). For new deployments, we recommend using the Python 3.9 Shared Library images. For existing deployments, we recommend migrating to those images.

Those currently using the container images published by [BC Gov on Docker Hub](https://hub.docker.com/r/bcgovimages/aries-cloudagent) should change to use those published to the [Hyperledger Package Repository under aries-cloudagent-python].

[Hyperledger Package Repository under aries-cloudagent-python]: https://github.com/orgs/hyperledger/packages?repo_name=aries-cloudagent-python
[publish.yml]: https://github.com/hyperledger/aries-cloudagent-python/blob/main/.github/workflows/publish.yml
[publish-indy.yml]: https://github.com/hyperledger/aries-cloudagent-python/blob/main/.github/workflows/publish-indy.yml
[Container Images and Github Actions]: https://github.com/hyperledger/aries-cloudagent-python/blob/main/ContainerImagesAndGithubActions.md

### Breaking Changes and Upgrades

**BREAKING** PR [\#2034](https://github.com/hyperledger/aries-cloudagent-python/pull/2034) -- Implicit connections
The break impacts existing deployments that support implicit connections, those initiated by another agent using a Public DID for this instance instead of an explicit invitation. Such deployments need to add the configuration parameter --requests-through-public-did to continue to support that feature. The use case is that an ACA-Py instance publishes a public DID on a ledger with a DIDComm service in the DIDDoc. Other agents resolve that DID, and attempt to establish a connection with the ACA-Py instance using the service endpoint. This is called an "implicit" connection in [RFC 0023 DID Exchange](https://github.com/hyperledger/aries-rfcs/blob/main/features/0023-did-exchange/README.md).

**BREAKING** PR [\#1913](https://github.com/hyperledger/aries-cloudagent-python/pull/1913) -- Unrevealed attributes in presentations
Updates the handling of "unrevealed attributes" during verification of AnonCreds presentations, allowing them to be used in a presentation, with additional data that can be checked if for unrevealed attributes. As few implementations of Aries wallets support unrevealed attributes in an AnonCreds presentation, this is unlikely to impact any deployments.

**BREAKING** PR [\#2145](https://github.com/hyperledger/aries-cloudagent-python/pull/2145) - Update webhook message to terse form by default, added startup flag --debug-webhooks for full form
The default behavior in ACA-Py has been to keep the full text of all messages in the protocol state object, and include the full protocol state object in the webhooks sent to the controller. When the messages include an object that is very large in all the messages, the webhook may become too big to be passed via HTTP. For example, issuing a credential with a photo as one of the claims may result in a number of copies of the photo in the protocol state object and hence, very large webhooks. This change reduces the size of the webhook message by eliminating redundant data in the protocol state of the "Issue Credential" message as the default, and adds a new parameter to use the old behavior.

**UPGRADE** PR [\#2116](https://github.com/hyperledger/aries-cloudagent-python/pull/2116) - UPGRADE: Fix multi-use invitation performance
The way that multiuse invitations in previous versions of ACA-Py caused performance to degrade over time. An update was made to add state into the tag names that eliminated the need to scan the tags when querying storage for the invitation.

If you are using multiuse invitations in your existing (pre-0.8.0 deployment of ACA-Py, you can run an upgrade to apply this change. To run upgrade from previous versions, use the following command using the 0.8.0 version of ACA-Py, adding you wallet settings:

`aca-py upgrade <other wallet config settings> --from-version=v0.7.5 --upgrade-config-path ./upgrade.yml`

## What's Changed
* feat: event and webhook on keylist update stored by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1769
* fix: warnings in tests from IndySdkProfile by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1865
* feat: make base wallet route access configurable by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1836
* Indy ledger fixes and cleanups by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1870
* Enable manually triggering keylist updates during connection by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1851
* Unit test fixes for python 3.9 by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1858
* feat: add universal resolver by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1866
* Allow fully qualified class names for profile managers by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/1880
* fix: didx request cannot be accepted by @rmnre in https://github.com/hyperledger/aries-cloudagent-python/pull/1881
* fix: resolve dids following new endpoint rules by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1863
* fix: unable to use askar with in memory db by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1878
* Refactoring of revocation registry creation by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1813
* Fixes a few AATH failures by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1897
* Refactor ledger correction code and insert into revocation error handling by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1892
* fix: update RouteManager methods use to pass profile as parameter by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/1902
* Update for the v1.0.0-rc0 release. Changelog comment added for v0.7.4 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1904
* Add seed command line parameter but use only if also an "allow insecure seed" parameter is set by @DaevMithran in https://github.com/hyperledger/aries-cloudagent-python/pull/1714
* Create sonarcloud.yml by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1910
* [#1895] Stopping the aca-py shell process keeps python process running by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1911
* Feat/public did endpoints for agents behind mediators by @cjhowland in https://github.com/hyperledger/aries-cloudagent-python/pull/1899
* Use did:key for recipient keys by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1886
* Revert "[#1895] Stopping the aca-py shell process keeps python process running" by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1916
* chore: update pydid by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1915
* fix: incorrect response schema for discover features by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1912
* Remove aca-py check for unrevealed revealed attrs on proof validation by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1913
* Fix: SchemasInputDescriptorFilter: broken deserialization renders generated clients unusable by @rmnre in https://github.com/hyperledger/aries-cloudagent-python/pull/1894
* Simple did registry by @burdettadam in https://github.com/hyperledger/aries-cloudagent-python/pull/1920
* Fix: the type of tails file path to string. by @baegjae in https://github.com/hyperledger/aries-cloudagent-python/pull/1925
* fix: propagate endpoint from mediation record by @cjhowland in https://github.com/hyperledger/aries-cloudagent-python/pull/1922
* Endorser doc updates and some bug fixes by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1926
* Send webhooks upon record/credential deletion by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1906
* Pre-populate revoc_reg_id on IssuerRevRegRecord by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/1924
* Delete sonarcloud.yml by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1935
* Fix/endpoint attrib structure by @cjhowland in https://github.com/hyperledger/aries-cloudagent-python/pull/1934
* fix: failed connectionless proof request on some case by @kukgini in https://github.com/hyperledger/aries-cloudagent-python/pull/1933
* Update pip-audit.yml by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1944
* Update pip-audit.yml by @ryjones in https://github.com/hyperledger/aries-cloudagent-python/pull/1945
* Fix: OOB - Handling of minor versions by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1940
* fix: Safely shutdown when root_profile uninitialized by @frostyfrog in https://github.com/hyperledger/aries-cloudagent-python/pull/1960
* feat: 00B v1.1 support by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1962
* Fix: `--mediator-invitation` with OOB invitation + cleanup  by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1970
* Fix: web.py dependency - integration tests & demos by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1973
* Leave credentialStatus element in the LD credential by @tsabolov in https://github.com/hyperledger/aries-cloudagent-python/pull/1921
* Author demo by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1975
* Endorser write DID transaction by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1938
* include image_url in oob invitation by @Zzocker in https://github.com/hyperledger/aries-cloudagent-python/pull/1966
* Fixed bug in run_demo script by @pasquale95 in https://github.com/hyperledger/aries-cloudagent-python/pull/1982
* chore: fix ACAPY_PROMOTE-AUTHOR-DID flag  by @morrieinmaas in https://github.com/hyperledger/aries-cloudagent-python/pull/1978
* fix: schema class can set Meta.unknown by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1885
* feat: update pynacl version from 1.4.0 to 1.50 by @morrieinmaas in https://github.com/hyperledger/aries-cloudagent-python/pull/1981
* did method & key type registry by @burdettadam in https://github.com/hyperledger/aries-cloudagent-python/pull/1986
* feat: include connection ids in keylist update webhook by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1914
* Fixes to acme exercise code by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1990
* Fix/txn job setting by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/1994
* Add 0.7.5 patch Changelog entry to main branch Changelog by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/1996
* Redis Plugins [redis_cache & redis_queue] related updates by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/1937
* Changelog and other updates for ACA-Py 1.0.0-rc1 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2005
* Fix typos in alice-local.sh & faber-local.sh by @naonishijima in https://github.com/hyperledger/aries-cloudagent-python/pull/2010
* fix: return if return route but no response by @TimoGlastra in https://github.com/hyperledger/aries-cloudagent-python/pull/1853
* Added a bit about manually creating a revoc reg tails file by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2012
* Fix for mediator load testing race condition when scaling horizontally by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2009
* Multi-ledger/Multi-tenant issues by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2022
* Dock updates for json demo by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2026
* fix: Correct typo in model -- required spelled incorrectly by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2031
* Feature: enabled handling VPs (request, creation, verification) with different VCs by @teanas in https://github.com/hyperledger/aries-cloudagent-python/pull/1956
* fix: update issue-credential endpoint summaries by @PeterStrob in https://github.com/hyperledger/aries-cloudagent-python/pull/1997
* Add ability to set docker container name by @matrixik in https://github.com/hyperledger/aries-cloudagent-python/pull/2024
* Code formatting by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2053
* ci: add gha for pr-tests by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2058
* Additional integration tests for revocation scenarios by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2055
* ci: test additional versions of python nightly by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2059
* Special handling for the write ledger by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2030
* #2041 - Issue JSON-LD has invalid Admin API documentation by @jfblier-amplitude in https://github.com/hyperledger/aries-cloudagent-python/pull/2046
* fix: indy dependency version format by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2054
* Add missing --mediator-connections-invite cmd arg info to docs by @matrixik in https://github.com/hyperledger/aries-cloudagent-python/pull/2051
* Do not reject OOB invitation with unknown handshake protocol(s) by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2060
* Update github actions dependencies (for node16 support) by @andrewwhitehead in https://github.com/hyperledger/aries-cloudagent-python/pull/2066
* fix: public did mediator routing keys as did keys by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/1977
* Improved validation of record attributes by @rmnre in https://github.com/hyperledger/aries-cloudagent-python/pull/2071
* BREAKING: Allow multi-use public invites and public invites with metadata by @mepeltier in https://github.com/hyperledger/aries-cloudagent-python/pull/2034
* feat: enable creation of DIDs for all registered methods by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2067
* Issue #2068 boolean flag change by @johnekent in https://github.com/hyperledger/aries-cloudagent-python/pull/2077
* fix claim format designation in presentation submission by @rmnre in https://github.com/hyperledger/aries-cloudagent-python/pull/2013
* Docker images and GHA for publishing images by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2076
* Allow using YAML configuration file with run_docker by @matrixik in https://github.com/hyperledger/aries-cloudagent-python/pull/2091
* fix: create local DID return schema by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2086
* feat: universal resolver - configurable authentication by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2095
* fix: fix connection timing bug by @reflectivedevelopment in https://github.com/hyperledger/aries-cloudagent-python/pull/2099
* Updating base images from slim-buster to slim-bullseye by @pradeepp88 in https://github.com/hyperledger/aries-cloudagent-python/pull/2105
* Multitenancy demo (docker-compose with postgres and ngrok) by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2089
* Update dockerfiles to use python 3.9 by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2109
* fix: resolver api schema inconsistency by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2112
* 0.8.0-rc0 release updates by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2115
* Fix publish workflows by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2117
* Fix ACA-py image builds by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2123
* Add startup flag --light-weight-webhook to trim down outbound webhook payload by @victorlee0505 in https://github.com/hyperledger/aries-cloudagent-python/pull/1941
* Delete tail files by @ramreddychalla94 in https://github.com/hyperledger/aries-cloudagent-python/pull/2103
* Update some of the demo Readme and Endorser instructions by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2122
* Respect `auto-verify-presentation` flag in present proof v1 and v2 by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2097
* Temporarily disable multi-architecture image builds by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2125
* OpenAPI validation fixes by @loneil in https://github.com/hyperledger/aries-cloudagent-python/pull/2127
* UPGRADE: Fix multi-use invitation performance by @reflectivedevelopment in https://github.com/hyperledger/aries-cloudagent-python/pull/2116
* Update ACA-Py docker files to produce OpenShift compatible images by @WadeBarnes in https://github.com/hyperledger/aries-cloudagent-python/pull/2130
* fix: response type on delete-tails-files endpoint by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2133
* Initial plugin docs by @ianco in https://github.com/hyperledger/aries-cloudagent-python/pull/2138
* feat: add verification method issue-credentials-2.0/send endpoint by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2135
* [fix] Removes extra comma that prevents swagger from accepting the presentation request by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2149
* Fix: Performance Demo [no --revocation] by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2151
* feat: allow marking non-SOV DIDs as public by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2144
* Update webhook message to terse form by default, added startup flag --debug-webhooks for full form by @victorlee0505 in https://github.com/hyperledger/aries-cloudagent-python/pull/2145
* fix: askar exception message always displaying null DID by @chumbert in https://github.com/hyperledger/aries-cloudagent-python/pull/2155
* Remove CircleCI Status since we aren't using CircleCI anymore by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2163
* Fix: messages stuck in mediator by @shaangill025 in https://github.com/hyperledger/aries-cloudagent-python/pull/2147
* 0.8.0 release by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2169

## New Contributors
* @cjhowland made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1899
* @kukgini made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1933
* @tsabolov made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1921
* @Zzocker made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1966
* @pasquale95 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1982
* @morrieinmaas made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1978
* @naonishijima made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2010
* @teanas made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1956
* @PeterStrob made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1997
* @matrixik made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2024
* @jfblier-amplitude made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2046
* @johnekent made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2077
* @pradeepp88 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2105
* @victorlee0505 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/1941
* @ramreddychalla94 made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2103
* @loneil made their first contribution in https://github.com/hyperledger/aries-cloudagent-python/pull/2127

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.7.5...0.8.0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.8.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-03-15 20:55:54 +0000 UTC
    </span>
</div>

