---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1523" class=".btn">#1523</a>
            </td>
            <td>
                <b>
                    downgrade npm on publish as temp fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                downgrade the version of npm on the publish step to ensure that publish doesn't give an ENOWORKSPACES error

This should be considered a temporary solution to getting publish working again and a better solution needs to be found.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-26 10:29:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1520" class=".btn">#1520</a>
            </td>
            <td>
                <b>
                    Temporarily revert publish to using node 16.x to fix broken publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is more of a case of quickly dropping down to an older version of `npm` so that it will fix the publish action.

Ideally we want to move to a supported version of node and address the issue that comes with that version of npm to perform a publish. It could be

1. move to an older version of npm (ie that one that comes with node 16), but this is not ideal
2. move to a newer version of npm as it may be an issue with the version that came with node 18, but this isn't likely
3. look at the npm publish command to see what needs to be done to make it work.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-25 13:23:37 +0000 UTC
    </div>
</div>

