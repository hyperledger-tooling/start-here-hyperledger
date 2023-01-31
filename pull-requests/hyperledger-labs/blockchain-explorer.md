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
                
            </td>
            <td>
                Signed-off-by: Abhay Kishore <abhay.kishore@walmart.com>

#### What this PR does / why we need it: It will purge the old data present in explorer db based on the parameter 'blockCount'

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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    added github ci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Aditya Joshi <adityaprakashjoshi1@gmail.com>

<!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
This PR has changes for adding github actions as CI. This will ensure the build and test are running fine.
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #329 

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
        Created At 2023-01-27 07:05:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/338" class=".btn">#338</a>
            </td>
            <td>
                <b>
                    BE 334 fetch data by block number, block range and transaction - Backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Anusha <anu.vp.nair@gmail.com>

<!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
This functionality enables the explorer to retrieve data using block id, block range (for example, blocks 1 to 10), and transaction data by giving the transaction id .Using these inputs, matching data are pulled in accordance with the user's search selection. First it will check whether the data is available in the PostgreSQL, if it is there it will fetch from there, otherwise it will fetch from blockchain.

With this new feature, data is fetched from the blockchain if it is not available in PostgreSQL using the block number, block number range, or transaction id.

#### Which issue(s) this PR fixes:

<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #334 

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note
 NONE
```

#### Additional documentation, usage docs, etc.:

<!--
This section can be blank if this pull request does not require a release note.

When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.


-->
```
http://<host>:<port>/api/fetchDataByBlockNo/:channel_genesis_hash/:blockNo
http://<host>:<port>/api/fetchDataByBlockRange/:channel_genesis_hash/:startBlockNo/:endBlockNo
http://<host>:<port>/api/fetchDataByTxnId/:channel_genesis_hash/:txnId
_Note_ : As part of testing, please pass bearer token for authorization
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-25 12:57:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/337" class=".btn">#337</a>
            </td>
            <td>
                <b>
                    BE-331 Display health status of peers and orderers- Backend
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
This feature enables the explorer to indicate the health status of peers and orderers that are online or offline.
As of now the explorer is not showing the status of peers/orderers that are part of HLF-Network. With this new feature enablement, we could display the health status of peers/orderers in the explorer dashboard.
#### Which issue(s) this PR fixes:
Fixes #331
<!-- 
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->


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
This functionality can be tested using the reqURL:
`http://<host>:<port>/api/peersStatus/:channel`
_Note_ : As part of testing, please pass bearer token for authorization
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
        Created At 2023-01-25 09:14:25 +0000 UTC
    </div>
</div>

