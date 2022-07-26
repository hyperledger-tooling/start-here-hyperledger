---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/936" class=".btn">#936</a>
            </td>
            <td>
                <b>
                    Update roadmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the road map for Solang and includes the newest additions and future features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 13:13:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/931" class=".btn">#931</a>
            </td>
            <td>
                <b>
                    Update substrate integration test environment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR upgrades the Substrate integration tests to work with an up-to-date Substrate runtime. The individual commits resemble more or less the steps needed to make this work. In summary:
* Switched to the `pullparitytech/contracts-ci-linux:production` image for having a node that will always be up-to-date
* Bump many npm deps in the testing frameworks
* Fix all test specs so the work again with the new runtime and updated deps
* Disable discovered regressions to make the GHA job pass

The regressions are most likely all related to issue #666. As discussed in today's stand up call, the plan is the following:
1. [In this PR] Update the integration test suite to work with current Substrate runtime, disabling any regressions related to runtime changes. This will let us continue to have a green CI setup on main. Based on that, a note in our `README.md` transparently informs what is not working and that we are aware.
2. Priority is on fixing issue #666 (and other potential metadata issues that may be discovered). Ideally this fixes all regressions.
3. Re-enable all tests that were disabled in this PR.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 16:00:35 +0000 UTC
    </div>
</div>

