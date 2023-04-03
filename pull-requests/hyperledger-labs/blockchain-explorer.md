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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/370" class=".btn">#370</a>
            </td>
            <td>
                <b>
                    Update Dockerfile
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
This PR fixes the bug related to Dockerfile 
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #369 

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
        Created At 2023-03-29 15:19:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    Frontend- Display chaincode metadata in chaincodes tab
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
The addition of a new feature in the Chaincodes tab that opens a dialogue model to show the details related to particular Chaincode. The new feature provides quick and easy access to important information related to the Chaincode.
With the new feature being added to the application, user can now have more visibility into the smart contracts they are using. One such feature is the ability to view the structure of the contract and its associated metadata information

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #367

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
```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 10:54:06 +0000 UTC
    </div>
</div>

