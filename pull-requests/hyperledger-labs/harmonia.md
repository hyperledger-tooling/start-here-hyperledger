---
layout: default
title: harmonia
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/harmonia
---

# harmonia <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/harmonia){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/50" class=".btn">#50</a>
            </td>
            <td>
                <b>
                    Enable wiki in code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Please make these changes in code, not the web UI :)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-23 13:12:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/harmonia/pull/49" class=".btn">#49</a>
            </td>
            <td>
                <b>
                    Fix build issue regarding Gradle repository declarations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Overview:**
Due to a change in R3s Artifactory usage, a number of repository declarations need to be updated as these locations are no longer available without authentication. However, an alternative public mirror is now available. 

**Changes:**
All references to `https://software.r3.com/artifactory`  changed to `https://download.corda.net/maven`. This is a public mirror of the previously available repository with access to the same artifacts.

`repositories.gradle` - updated to reference `https://download.corda.net/maven/corda-dependencies`, rather than the previous `*/corda` repository, the reason for this is `corda` is a virtual repository in artifactory consisting of several others, this concept of a virtual repository does not exist in the public mirror, so we explicitly declare the needed repository.

Local compilation is confirmed to be working as expected with this change


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 13:46:10 +0000 UTC
    </div>
</div>

