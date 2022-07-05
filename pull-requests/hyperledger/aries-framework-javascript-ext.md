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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    refactor(react-hooks): update AFJ to stable 0.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes a refactor of the current react-hooks extension including:
* Updated AFJ dependency to the official 0.2.0 release
* Base record events are now handled as opposed to events for each specific record type
* Introduces a typed reducer hook factory to handle record actions in providers
* Uses agent event observable stream to allow for introduction of rxjs operators
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 03:40:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/135" class=".btn">#135</a>
            </td>
            <td>
                <b>
                    chore: release @aries-framework/redux-store 0.3.0
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
## [0.3.0](https://www.github.com/hyperledger/aries-framework-javascript-ext/compare/redux-store-v0.2.0...redux-store-v0.3.0) (2022-07-04)


### ⚠ BREAKING CHANGES

* **redux-store:** The thunks that exposed all module methods from AFJ are now removed. Instead of using the thunks, you should use the agent directly.

### Features

* **redux-store:** update to afj 0.2.0 ([#133](https://www.github.com/hyperledger/aries-framework-javascript-ext/issues/133)) ([969ab1f](https://www.github.com/hyperledger/aries-framework-javascript-ext/commit/969ab1f167923f70e5f3441679d5de97af922282))
---


This PR was generated with [Release Please](https://github.com/googleapis/release-please). See [documentation](https://github.com/googleapis/release-please#release-please).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 11:29:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/134" class=".btn">#134</a>
            </td>
            <td>
                <b>
                    chore: nohoist afj dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Multiple version of AFJ is causing issues, this gives every packages in this repo their own version of AFJ (so they can depend on different AFJ versions). Hope to be able to remove this once all packages are updated.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-04 11:07:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/133" class=".btn">#133</a>
            </td>
            <td>
                <b>
                    feat(redux-store)!: update to afj 0.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates redux store package to AFJ 0.2.0, removes most of the thunks (except get all to initialize the state) and updates the event listeners to the generic record events.

Supersedes #119.

MAKE SURE TO ADD THE FOLLOWING BREAKING CHANGES TO THE END OF THE SQUASHED COMMIT MESSAGE:

BREAKING CHANGE: the state changed events listeners have been updated to the new generic record saved/updated/deleted events. Instead of using a listener for each of the record types, you only have to use the `startRecordsListeners` method now.

BREAKING CHANGE: The thunks that exposed all module methods from AFJ are now removed. Instead of using the thunks, you should use the agent directly.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-03 13:20:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/132" class=".btn">#132</a>
            </td>
            <td>
                <b>
                    chore: release @aries-framework/react-hooks 0.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">autorelease: pending</span>
            </td>
            <td>
                :robot: I have created a release \*beep\* \*boop\*
---
## [0.3.0](https://www.github.com/hyperledger/aries-framework-javascript-ext/compare/react-hooks-v0.2.0...react-hooks-v0.3.0) (2022-07-04)


### ⚠ BREAKING CHANGES

* **react-hooks:** `useConnectionByState` now needs a `DidExchangeState` state value instead of a `ConnectionState` state value.

### Bug Fixes

* **react-hooks:** update providers on delete events ([#113](https://www.github.com/hyperledger/aries-framework-javascript-ext/issues/113)) ([d1e5292](https://www.github.com/hyperledger/aries-framework-javascript-ext/commit/d1e52929275e69c963bb0dd35a878aba4f250bd9))
---


This PR was generated with [Release Please](https://github.com/googleapis/release-please). See [documentation](https://github.com/googleapis/release-please#release-please).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 14:46:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    chore: release @aries-framework/push-notifications 0.4.0
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
## [0.4.0](https://www.github.com/hyperledger/aries-framework-javascript-ext/compare/push-notifications-v0.3.0...push-notifications-v0.4.0) (2022-06-28)


### ⚠ BREAKING CHANGES

* **push-notifications:** update to afj 0.2.0 (#126)

### Features

* **push-notifications:** update to afj 0.2.0 ([#126](https://www.github.com/hyperledger/aries-framework-javascript-ext/issues/126)) ([196a323](https://www.github.com/hyperledger/aries-framework-javascript-ext/commit/196a3233f7284ed2acdba9d3724acc5c55cd2be4))


### Bug Fixes

* **push-notifications:** validation method ([f8b9c1b](https://www.github.com/hyperledger/aries-framework-javascript-ext/commit/f8b9c1b1d18780227b7db6a30efe11f407da5ef3))
---


This PR was generated with [Release Please](https://github.com/googleapis/release-please). See [documentation](https://github.com/googleapis/release-please#release-please).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 14:46:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    chore: merge afj-0.2.0 into main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Merge afj-0.2.0 into main now that 0.2.0 has been released
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 14:06:13 +0000 UTC
    </div>
</div>

