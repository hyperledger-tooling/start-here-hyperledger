---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1505" class=".btn">#1505</a>
            </td>
            <td>
                <b>
                    Update manifest with evmconnect 1.3.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 10:42:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1504" class=".btn">#1504</a>
            </td>
            <td>
                <b>
                    Upgrade psql client dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should fix the failing docker build
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 19:15:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1503" class=".btn">#1503</a>
            </td>
            <td>
                <b>
                    Move doc site to new Hyperledger template
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the doc site to use the new Hyperledger recommended framework using `mkdocs` and GitHub Pages. It uses a plugin called `mike` to manage the versions
- GitHub workflows have been updated to use this new build as well
-  All of this should fix the problem we always had when someone released a hotfix release for an older version of FireFly it  messed up the docs site in the past, because the concept of `latest` was ambiguous
- I've backported the docs for one previous release v1.2.2 into the new framework so it shows up in the version list. If we feel like we need more than that, we can do additional releases, but it's a bit of manual work

New version of the doc site is live at: https://hyperledger.github.io/firefly/latest/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 18:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1502" class=".btn">#1502</a>
            </td>
            <td>
                <b>
                    Send start msg on reconnect for token connectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When the token connector is restarted, it needs to be sent the start namespace message 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 15:25:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1501" class=".btn">#1501</a>
            </td>
            <td>
                <b>
                    Add base API url to contract api result
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes https://github.com/hyperledger/firefly/issues/1500
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 11:06:27 +0000 UTC
    </div>
</div>

