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
                    1.0.0-rc1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    1.0.0-rc1
                </span>
            </td>
            <td>
                1.0.0 is a breaking update to ACA-Py whose version is intended to indicate the
maturity of the implementation. The final 1.0.0 release will be Aries Interop
Profile 2.0-complete, and based on Python 3.7 or higher.

In rc1, there are not a lot of new features, as the focus is on cleanup and
optimization. The biggest is the inclusion with ACA-Py of a universal resolver
interface, allowing an instance to have both local resolvers for some DID
Methods and a call out to an external universal resolver for other DID Methods.
Another significant feature is full support for Hyperledger Indy transaction
endorsement for Authors and Endorsers. A new repo
[aries-endorser-service](https://github.com/hyperledger/aries-endorser-service)
has been created that is a pre-configured instance of ACA-Py for use as an
Endorser service. While some work has been done on moving the default Python
version beyond 3.6, more work is still to be done on that before the final
v1.0.0 release.

### Breaking Changes

As of release candidate 1.0.0-rc1, the only identified breaking change is the
handling of "unrevealed attributes" during verification (see
[\#1913](https://github.com/hyperledger/aries-cloudagent-python/pull/1913) for
details). As few implementations of Aries Wallets support unrevealed attributes
in an AnonCreds presentation, this is unlikely to impact any deployments.

### What's Changed Since 1.0.0-rc0

See the [Changelog for v1.0.0-rc1](https://github.com/hyperledger/aries-cloudagent-python/blob/1.0.0-rc1/CHANGELOG.md#100-rc1) for all changes since v0.7.4.

- Add 0.7.5 patch Changelog entry to main branch Changelog [\#1996](https://github.com/hyperledger/aries-cloudagent-python/pull/1996) ([swcurran](https://github.com/swcurran))
- Fix/txn job setting [\#1994](https://github.com/hyperledger/aries-cloudagent-python/pull/1994) ([ianco](https://github.com/ianco))
- Fixes to acme exercise code [\#1990](https://github.com/hyperledger/aries-cloudagent-python/pull/1990) ([ianco](https://github.com/ianco))
- did method & key type registry [\#1986](https://github.com/hyperledger/aries-cloudagent-python/pull/1986) ([burdettadam](https://github.com/burdettadam))
- Fixed bug in run\_demo script [\#1982](https://github.com/hyperledger/aries-cloudagent-python/pull/1982) ([pasquale95](https://github.com/pasquale95))
- feat: update pynacl version from 1.4.0 to 1.50 [\#1981](https://github.com/hyperledger/aries-cloudagent-python/pull/1981) ([morrieinmaas](https://github.com/morrieinmaas))
- chore: fix ACAPY\_PROMOTE-AUTHOR-DID flag  [\#1978](https://github.com/hyperledger/aries-cloudagent-python/pull/1978) ([morrieinmaas](https://github.com/morrieinmaas))
- Author demo [\#1975](https://github.com/hyperledger/aries-cloudagent-python/pull/1975) ([ianco](https://github.com/ianco))
- Fix: web.py dependency - integration tests & demos [\#1973](https://github.com/hyperledger/aries-cloudagent-python/pull/1973) ([shaangill025](https://github.com/shaangill025))
- Fix: `--mediator-invitation` with OOB invitation + cleanup  [\#1970](https://github.com/hyperledger/aries-cloudagent-python/pull/1970) ([shaangill025](https://github.com/shaangill025))
- include image\_url in oob invitation [\#1966](https://github.com/hyperledger/aries-cloudagent-python/pull/1966) ([Zzocker](https://github.com/Zzocker))
- feat: 00B v1.1 support [\#1962](https://github.com/hyperledger/aries-cloudagent-python/pull/1962) ([shaangill025](https://github.com/shaangill025))
- fix: Safely shutdown when root\_profile uninitialized [\#1960](https://github.com/hyperledger/aries-cloudagent-python/pull/1960) ([frostyfrog](https://github.com/frostyfrog))
- Update pip-audit.yml [\#1945](https://github.com/hyperledger/aries-cloudagent-python/pull/1945) ([ryjones](https://github.com/ryjones))
- Update pip-audit.yml [\#1944](https://github.com/hyperledger/aries-cloudagent-python/pull/1944) ([ryjones](https://github.com/ryjones))
- Fix: OOB - Handling of minor versions [\#1940](https://github.com/hyperledger/aries-cloudagent-python/pull/1940) ([shaangill025](https://github.com/shaangill025))
- Endorser write DID transaction [\#1938](https://github.com/hyperledger/aries-cloudagent-python/pull/1938) ([ianco](https://github.com/ianco))
- Redis Plugins \[redis\_cache & redis\_queue\] related updates [\#1937](https://github.com/hyperledger/aries-cloudagent-python/pull/1937) ([shaangill025](https://github.com/shaangill025))
- Delete sonarcloud.yml [\#1935](https://github.com/hyperledger/aries-cloudagent-python/pull/1935) ([ryjones](https://github.com/ryjones))
- Fix/endpoint attrib structure [\#1934](https://github.com/hyperledger/aries-cloudagent-python/pull/1934) ([cjhowland](https://github.com/cjhowland))
- fix: failed connectionless proof request on some case [\#1933](https://github.com/hyperledger/aries-cloudagent-python/pull/1933) ([kukgini](https://github.com/kukgini))
- Endorser doc updates and some bug fixes [\#1926](https://github.com/hyperledger/aries-cloudagent-python/pull/1926) ([ianco](https://github.com/ianco))
- Fix: the type of tails file path to string. [\#1925](https://github.com/hyperledger/aries-cloudagent-python/pull/1925) ([baegjae](https://github.com/baegjae))
- Pre-populate revoc\_reg\_id on IssuerRevRegRecord [\#1924](https://github.com/hyperledger/aries-cloudagent-python/pull/1924) ([andrewwhitehead](https://github.com/andrewwhitehead))
- fix: propagate endpoint from mediation record [\#1922](https://github.com/hyperledger/aries-cloudagent-python/pull/1922) ([cjhowland](https://github.com/cjhowland))
- Leave credentialStatus element in the LD credential [\#1921](https://github.com/hyperledger/aries-cloudagent-python/pull/1921) ([tsabolov](https://github.com/tsabolov))
- Simple did registry [\#1920](https://github.com/hyperledger/aries-cloudagent-python/pull/1920) ([burdettadam](https://github.com/burdettadam))
- Revert "\[\#1895\] Stopping the aca-py shell process keeps python process running" [\#1916](https://github.com/hyperledger/aries-cloudagent-python/pull/1916) ([ryjones](https://github.com/ryjones))
- chore: update pydid [\#1915](https://github.com/hyperledger/aries-cloudagent-python/pull/1915) ([dbluhm](https://github.com/dbluhm))
- feat: include connection ids in keylist update webhook [\#1914](https://github.com/hyperledger/aries-cloudagent-python/pull/1914) ([dbluhm](https://github.com/dbluhm))
- Remove aca-py check for unrevealed revealed attrs on proof validation [\#1913](https://github.com/hyperledger/aries-cloudagent-python/pull/1913) ([ianco](https://github.com/ianco))
- fix: incorrect response schema for discover features [\#1912](https://github.com/hyperledger/aries-cloudagent-python/pull/1912) ([dbluhm](https://github.com/dbluhm))
- \[\#1895\] Stopping the aca-py shell process keeps python process running [\#1911](https://github.com/hyperledger/aries-cloudagent-python/pull/1911) ([ryjones](https://github.com/ryjones))
- Create sonarcloud.yml [\#1910](https://github.com/hyperledger/aries-cloudagent-python/pull/1910) ([ryjones](https://github.com/ryjones))
- Send webhooks upon record/credential deletion [\#1906](https://github.com/hyperledger/aries-cloudagent-python/pull/1906) ([frostyfrog](https://github.com/frostyfrog))
- Feat/public did endpoints for agents behind mediators [\#1899](https://github.com/hyperledger/aries-cloudagent-python/pull/1899) ([cjhowland](https://github.com/cjhowland))
- Fix: SchemasInputDescriptorFilter: broken deserialization renders generated clients unusable [\#1894](https://github.com/hyperledger/aries-cloudagent-python/pull/1894) ([rmnre](https://github.com/rmnre))
- Use did:key for recipient keys [\#1886](https://github.com/hyperledger/aries-cloudagent-python/pull/1886) ([frostyfrog](https://github.com/frostyfrog))
- fix: schema class can set Meta.unknown [\#1885](https://github.com/hyperledger/aries-cloudagent-python/pull/1885) ([dbluhm](https://github.com/dbluhm))
- Add seed command line parameter but use only if also an "allow insecure seed" parameter is set [\#1714](https://github.com/hyperledger/aries-cloudagent-python/pull/1714) ([DaevMithran](https://github.com/DaevMithran))

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/1.0.0-rc1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-11-04 22:25:54 +0000 UTC
    </span>
</div>

