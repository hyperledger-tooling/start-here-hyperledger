---
layout: default
title: besu
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.7.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.6
                </span>
            </td>
            <td>
                ## 22.7.6
Hotfix release of the 22.7.x series to address [#4495](https://github.com/hyperledger/besu/issues/4495) which could result in failed block proposals on merge networks. Besu version 22.7.6 will automatically invalidate the bloomfilter cache from prior versions of besu and regenerate the cache in the background.

### Additions and Improvements
- Bring GraphQL into compliance with execution-api specs [#4112](https://github.com/hyperledger/besu/pull/4112)

### Bug Fixes
- Corrects emission of blockadded events when rewinding during a re-org. [#4497](https://github.com/hyperledger/besu/issues/4497)

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.6/besu-22.7.6.zip / sha256: ae05040027b96ba458a08cfee8577dafe1d85a3afce793f00f798cedb3ab547d
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.6/besu-22.7.6.tar.gz / sha256: 9e538852f16fd39b884c4c342beaad813e33ab24890634c01eee3d37dc1da893

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.7.6" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-10-07 23:19:08 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.10.0-RC1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.10.0-RC1
                </span>
            </td>
            <td>
                ## 22.10.0-RC1

### Additions and Improvements
- Bring GraphQL into compliance with execution-api specs [#4112](https://github.com/hyperledger/besu/pull/4112)
- Improve UX of initial sync logs, pushing not relevant logs to debug level [#4486](https://github.com/hyperledger/besu/pull/4486)
- Refactor unverified forkchoice event [#4487](https://github.com/hyperledger/besu/pull/4487)
- Optimize pivot block selector on PoS networks [#4488](https://github.com/hyperledger/besu/pull/4488)
- Optimize Snap sync on PoS networks [#4462](https://github.com/hyperledger/besu/pull/4462)

### Bug Fixes

### Download Links
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.10.0-RC1/besu-22.10.0-RC1.zip / sha256: 16fd47533aa2986491143e5f4a052c0aa4866ebfa415abbf3ca868e4fbeac6ce
https://hyperledger.jfrog.io/artifactory/besu-binaries/besu/22.10.0-RC1/besu-22.10.0-RC1.tar.gz / sha256: 48fd3480e4380580ed9187302be987e9eca2b445935ec6a509e7269898d8a4a8

            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.10.0-RC1" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-10-06 23:53:31 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    22.7.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    22.7.5
                </span>
            </td>
            <td>
                
### Additions and Improvements
- Avoid sending added block events to transaction pool, and processing incoming transactions during initial sync [#4457](https://github.com/hyperledger/besu/pull/4457)
- When building a new proposal, keep the best block built until now instead of the last one [#4455](https://github.com/hyperledger/besu/pull/4455)
- Add Mainnet to merged networks [#4463](https://github.com/hyperledger/besu/pull/4463)

### Bug Fixes
- Fixed logIndex value returned by eth_getLogs RPC call [#4355](https://github.com/hyperledger/besu/pull/4355)

### Download Links
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.5/besu-22.7.5.zip / sha256: b5d7b255b249beea0f46ec397122823c75f2373083a71a9f7b4c98b2b0f94997
https://hyperledger.jfrog.io/hyperledger/besu-binaries/besu/22.7.5/besu-22.7.5.tar.gz / sha256: 91e3cbc16c46c53f7bf55bdd968553d0fb4087bff1e244cb03ac175ac54cf718


            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/besu/releases/tag/22.7.5" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-10-05 17:04:11 +0000 UTC
    </span>
</div>

