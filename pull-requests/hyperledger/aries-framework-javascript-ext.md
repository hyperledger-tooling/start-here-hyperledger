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

