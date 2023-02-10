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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2114" class=".btn">#2114</a>
            </td>
            <td>
                <b>
                    Feat: Multiple Presentations [v2.1]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - WIP, routes schema updates and complete unit test coverage pending
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-07 17:22:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2112" class=".btn">#2112</a>
            </td>
            <td>
                <b>
                    fix: resolver api schema inconsistency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix a small inconsistency between the openapi schema and the actual return value for the `/resolver/resolve/{did}`.

This PR aligns the schema to the actual return value to avoid breaking any current implementation making use of the endpoint.

Signed-off-by: Clément Humbert <clement.humbert@sicpa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 09:01:41 +0000 UTC
    </div>
</div>

