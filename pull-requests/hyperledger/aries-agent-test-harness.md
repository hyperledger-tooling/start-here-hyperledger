---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/372" class=".btn">#372</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 03:52:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    chore: update afj, remove setTimeouts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

- Updates AFJ to latest version (and also uses `latest` as version indicator). This means if a new version is released it should be picked up by the CI. This also means the AFJ backchannel will probably break more often, as we're still making a lot of breaking changes. I hope this will make sure I keep it up to date :)
- Removes the `setTimeouts` from the controller and instead uses events to know when we can take the next action (@nodlesh)
- @lauravuo-techlab it seems that updating AFJ fixed the issue with findy (yay! :)). On my local machine the following command (`./manage run -d javascript -b findy -t @AcceptanceTest -t @AIP10 -t ~@wip -t ~@revocation`) all tests succeeds



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-24 20:05:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/370" class=".btn">#370</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 03:52:22 +0000 UTC
    </div>
</div>

