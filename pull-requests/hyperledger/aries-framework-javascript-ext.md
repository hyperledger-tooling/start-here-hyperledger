---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/227" class=".btn">#227</a>
            </td>
            <td>
                <b>
                    chore: release @aries-framework/transport-ble 0.2.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">autorelease: tagged</span><span class="chip">ci-test</span>
            </td>
            <td>
                :robot: I have created a release \*beep\* \*boop\*
---
### [0.2.1](https://www.github.com/hyperledger/aries-framework-javascript-ext/compare/transport-ble-v0.2.0...transport-ble-v0.2.1) (2023-09-18)


### Bug Fixes

* loosen types on ble inbound and outbound transport and session ([#226](https://www.github.com/hyperledger/aries-framework-javascript-ext/issues/226)) ([17c6203](https://www.github.com/hyperledger/aries-framework-javascript-ext/commit/17c6203b398ad2fd613bc237e2c852a86f44c444))
---


This PR was generated with [Release Please](https://github.com/googleapis/release-please). See [documentation](https://github.com/googleapis/release-please#release-please).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 08:36:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/226" class=".btn">#226</a>
            </td>
            <td>
                <b>
                    fix: loosen types on ble inbound and outbound transport and session
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Types were unnecessarily strict and this loosens it a bit.
    - Now `Peripheral` and `Central` are both allowed for inbound and outbound as they both extend `Ble`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-18 07:43:05 +0000 UTC
    </div>
</div>

