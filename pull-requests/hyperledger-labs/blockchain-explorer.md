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
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/378" class=".btn">#378</a>
            </td>
            <td>
                <b>
                    Backend - Pagination implementation for Blocks Tab
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it: 
This feature implements the pagination for list of blocks to be fetched from PostgreSQL.
As of now the pagination is being handled from UI. Implementing pagination from backend addresses an issue when dealing with retrieval of huge data sets.

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #356

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note
No

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
        Created At 2023-04-04 10:35:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    Chaincode count on Dashboard is incorrect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
The Chaincode Names with various versions are visible in the UI. So here in order to get the chaincode count, it should be as per the number of distinct chaincodes installed. So, in current state we are not considering the versions of chaincodes.
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #373

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note
No
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
        Created At 2023-04-04 07:55:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/376" class=".btn">#376</a>
            </td>
            <td>
                <b>
                    Add validations to search functionality blockId and blockRange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
By adding validations, the code can handle the issues arising due to incorrect channelgenesishash etc. A user can also configure the "blockRangeLimit" in the config.json file. A backend configurable "blockRangeLimit" value can harness the user, with more flexibility of setting the blockRange value.
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #375

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
        Created At 2023-04-03 13:45:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    Empty org is being displayed while fetching the list of orgs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
Test the Explorer compatibility with Hyperledger Fabric v2.4.7.
The functionality which fetches the list of orgs, is also fetching an empty org. This is due to the reason that the first transaction of type "config" is not associated with any creator organisation. So, while saving this transaction to the postgres, the field creator_msp_id is blank.
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #372

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
        Created At 2023-04-03 07:36:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    Add Frontend blocks view pagination and block range search
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">do not merge</span><span class="chip">feature</span>
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:                    
This feature integrates the Api calls to render server-side pagination for list of Blocks to be fetched.
As of now the pagination is being handled from UI. Implementing pagination from backend addresses an issue when dealing with retrieval of huge data sets.

The Block Range Search feature facilitates user to search data using a block range. The Search field is provided in the blocks tab. A modal with the appropriate data will be displayed in response to user input.
It provisions user for a quick data search pertaining to specific block range.
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #355 and #365 

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note
Yes
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
        Created At 2023-03-30 10:46:17 +0000 UTC
    </div>
</div>

