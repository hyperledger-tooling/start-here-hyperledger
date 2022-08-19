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
                    1.0.0-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.0.0-rc0
                </span>
            </td>
            <td>
                1.0.0 is a breaking update to ACA-Py whose version is intended to indicate the maturity of the implementation. The final 1.0.0 release will be Aries Interop Profile 2.0-complete, and based on Python 3.7 or higher. The initial (rc0) release candidate is for early adopters to provide feedback.

See the [CHANGELOG.md](https://github.com/hyperledger/aries-cloudagent-python/blob/1.0.0-rc0/CHANGELOG.md) for the highlights in this release and a categorized list of pull requests.

### Breaking Changes

As of rc0, there are no breaking updates in the release from the previous v0.7.4. However, we know that there are some pending updates that will be breaking, hence the bumps to the major/minor version elements.

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


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.7.4...1.0.0-rc0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/1.0.0-rc0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-08-18 20:20:18 +0000 UTC
    </span>
</div>

