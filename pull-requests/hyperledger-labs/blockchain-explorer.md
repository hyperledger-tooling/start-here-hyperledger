---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    BE-340 Display health status of peers and orderers - FrontEnd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                …ity of peers and orderers

Signed-off-by: saksham1203 <saksham.s1203@gmail.com>

<!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
This feature enables the explorer to indicate the health status of peers and orderers that are online or offline.
The status can be indicated with red being offline, green being online, green with flickering - fetching status.
As of now the explorer is not showing the status of peers/orderers that are part of HLF-Network. With this new feature enablement, we could display the health status of peers/orderers in the explorer dashboard.

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #340 

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note
yes
```

#### Additional documentation, usage docs, etc.:

<!--
This section can be blank if this pull request does not require a release note.

When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.


-->

![peer status](https://user-images.githubusercontent.com/72246428/215970360-2f8e6a84-8846-484d-ba5b-d35f7f3851e6.png "peer status").

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 06:43:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Purge data in explorer based on a parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Abhay Kishore <abhay.kishore@walmart.com>

#### What this PR does / why we need it: 
It will purge the old data present in explorer db based on the parameter `blockCount`.`blockCount` property can be defined in `config.json`.

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note

```

#### Additional documentation, usage docs, etc.:

<!--
This section can be blank if this pull request does not require a release note.

When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.


-->
```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 09:40:01 +0000 UTC
    </div>
</div>

