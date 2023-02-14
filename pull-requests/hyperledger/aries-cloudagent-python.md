---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2120" class=".btn">#2120</a>
            </td>
            <td>
                <b>
                    Update demo to issue multiple credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

@swcurran / @shaangill025  this adds an option to the demo ("1m") to issue multiple creds, in either indy or json-ld format.

It includes all creds in one offer, rather than the verbose request/response protocol.

Let me know if there are other additions to the demo you would like.

(There is also a new integration test - it doesn't work yet but @swcurran said last week to not worry about integration tests yet ...)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 18:39:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2117" class=".btn">#2117</a>
            </td>
            <td>
                <b>
                    Fix publish workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Trigger when releases and prereleases are published.

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-11 13:16:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2116" class=".btn">#2116</a>
            </td>
            <td>
                <b>
                    Fix multi-use invitation performance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Multiuse invitation performance degrades over time. By adding state into the tag names, performance doesn't degrade over time while using multi-use invitations.

This breaks backwards compatibility, but while load testing it can be seen that performance no longer degrades when using a multi-use invitation. Previously, only 1600 connections could be established while load testing, and on a second run is reduced to 300. After the modification, the load testing exceeded 2400 connections and the testing client machine ran out of ram for clients.

This shows a clear improvement in performance.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-11 00:37:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2115" class=".btn">#2115</a>
            </td>
            <td>
                <b>
                    0.8.0-rc0 release updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates necessary to create a 0.8.0-rc0 release. For this release, the CHANGELOG.md has been update to move the categorized list of Pull Requests from the "0.1.0-rc1" to under this release, and then the PRs since 1.0.0-rc1 were added.

My proposal is that after we release 0.8.0 (final), we follow up with a 0.1.0-rc2 release that is the same as 0.8.0 so that those tracking to the 1.0.0 release can use that. As needed, we can do the same for 0.8.1 / 0.9.0 if needed, but ideally we will get 1.0.0 out the door before those are needed.

@WadeBarnes @ianco @dbluhm -- does that make sense?

Also, please review the note I put into the changelog about the container images (do we have link to put into that paragraph), and if what I state is accurate.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 00:01:50 +0000 UTC
    </div>
</div>

