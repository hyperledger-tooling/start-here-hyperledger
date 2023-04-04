---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2369" class=".btn">#2369</a>
            </td>
            <td>
                <b>
                    refactor(workflows): use 4vcpu runner for weaver data sharing workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is to resolve data sharing worklow failing for abritrary reasons.
Additionally rename weaver workflows jobs, so as to uniquely identify them by their name.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 16:56:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2368" class=".btn">#2368</a>
            </td>
            <td>
                <b>
                    chore(ci): update deprecated GitHub API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use current version of GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 15:50:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2366" class=".btn">#2366</a>
            </td>
            <td>
                <b>
                    fix: Upgrade dependencies in Cargo.toml file for cactus-plugin-keychain-vault package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …atements in cactus-plugin-keychain-vault package
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 12:33:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2363" class=".btn">#2363</a>
            </td>
            <td>
                <b>
                    feat(cactus-cmd-gui-app): extend common cacti gui app to operate with  fabric hyperledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add feature and options to switch in GUI app to visualize fabric hyperledger ledger data stored in supabase by persistence plugins

Depends on: https://github.com/hyperledger/cacti/pull/2265
Depends on: https://github.com/hyperledger/cacti/pull/2331

Signed-off-by: Barnaba Pawelczak [barnaba.pawelczak@fujitsu.com](mailto:barnaba.pawelczak@fujitsu.com)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 10:44:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2362" class=".btn">#2362</a>
            </td>
            <td>
                <b>
                    fix(weaver): address vulnerability CVE-2020-28477 and many others
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - https://github.com/hyperledger/cacti/security/dependabot/434
- https://github.com/hyperledger/cacti/security/dependabot/435
- https://github.com/hyperledger/cacti/security/dependabot/423
- https://github.com/hyperledger/cacti/security/dependabot/499
- https://github.com/hyperledger/cacti/security/dependabot/570
- https://github.com/hyperledger/cacti/security/dependabot/594
- https://github.com/hyperledger/cacti/security/dependabot/592
- https://github.com/hyperledger/cacti/security/dependabot/590
- https://github.com/hyperledger/cacti/security/dependabot/589
- https://github.com/hyperledger/cacti/security/dependabot/588
- https://github.com/hyperledger/cacti/security/dependabot/594
- https://github.com/hyperledger/cacti/security/dependabot/591
- Remove unwanted dependencies in `weaver-besu-sdk`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 06:48:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2359" class=".btn">#2359</a>
            </td>
            <td>
                <b>
                    fix(relay): rust build fails after tokio bump from 0.2.25 to 1.18.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    Additionally:
    - upgrade other dependencies for relay
    - added tls based unit test in relay

Closes #2349 

Replaces #2351 which I closed by accident
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 17:02:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2353" class=".btn">#2353</a>
            </td>
            <td>
                <b>
                    fix(interopcc): build failing after golang.org/x/crypto bump to v0.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    Upgraded all go modules to go v1.20
    
Closes #2348 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 18:21:33 +0000 UTC
    </div>
</div>

