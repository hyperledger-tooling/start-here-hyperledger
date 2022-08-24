---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.1.0-alpha.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.1.0-alpha.4
                </span>
            </td>
            <td>
                ## What's Changed
* Performance improvements for batch lookups by @awrichar in https://github.com/hyperledger/firefly/pull/967
* Messages that fail validation should be rejected by @awrichar in https://github.com/hyperledger/firefly/pull/956
* Update to firefly-signer v0.9.13 by @nguyer in https://github.com/hyperledger/firefly/pull/969
* Update to firefly-signer v0.9.15 by @nguyer in https://github.com/hyperledger/firefly/pull/970
* Fix group race condition, optimize transaction cache by @awrichar in https://github.com/hyperledger/firefly/pull/971
* fix integration matrix `exclude` by @shorsher in https://github.com/hyperledger/firefly/pull/973
* Add cache for operations by @awrichar in https://github.com/hyperledger/firefly/pull/972
* Adjust defaults for all cache items that don't expose a Size by @awrichar in https://github.com/hyperledger/firefly/pull/975
* Only query operations from the database if there were cache misses by @awrichar in https://github.com/hyperledger/firefly/pull/976
* Leverage transaction cache in a few more places by @awrichar in https://github.com/hyperledger/firefly/pull/974
* Use optimistic inserts for blockchain events by @awrichar in https://github.com/hyperledger/firefly/pull/977
* Create config migration script by @awrichar in https://github.com/hyperledger/firefly/pull/934
* Add nil check for blobReceiver during WaitStop by @awrichar in https://github.com/hyperledger/firefly/pull/980
* add nil check for aggregator during WaitStop by @shorsher in https://github.com/hyperledger/firefly/pull/981
* bump reset polling to 60seconds by @shorsher in https://github.com/hyperledger/firefly/pull/983
* Update firefly_node.md by @Liadc in https://github.com/hyperledger/firefly/pull/987
* Fix bugs when running with an old config file by @awrichar in https://github.com/hyperledger/firefly/pull/984
* Restore camelCase key names by @awrichar in https://github.com/hyperledger/firefly/pull/988
* Add /pins/rewind API for requesing manual rewind by @awrichar in https://github.com/hyperledger/firefly/pull/991
* Wait for server to exit, before restarting for reset by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/994
* Propagate the underlying parse error by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/992
* Do not rely on "topic" to be present in event streams by @awrichar in https://github.com/hyperledger/firefly/pull/999
* Manifest updates for v1.1.0-rc.1 by @peterbroadhurst in https://github.com/hyperledger/firefly/pull/1000

## New Contributors
* @Liadc made their first contribution in https://github.com/hyperledger/firefly/pull/987

**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.1.0-alpha.3...v1.1.0-alpha.4
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.1.0-alpha.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-08-23 22:08:59 +0000 UTC
    </span>
</div>

<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.0.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.0.4
                </span>
            </td>
            <td>
                ## What's Changed
* Misc cleanup for 1.0 branch by @awrichar in https://github.com/hyperledger/firefly/pull/982


**Full Changelog**: https://github.com/hyperledger/firefly/compare/v1.0.3...v1.0.4
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/firefly/releases/tag/v1.0.4" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-08-18 20:20:25 +0000 UTC
    </span>
</div>

