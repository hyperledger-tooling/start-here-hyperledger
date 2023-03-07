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
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/363" class=".btn">#363</a>
            </td>
            <td>
                <b>
                    maintainers contact
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                how to contact to maintainers details.

<!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:

Update on maintainer contact details know how.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-05 19:05:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    purge functionality based on blockcount and time
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

Now explorer database is saving each transaction that is committed on to the ledger making replica copies of ledger. When number of transactions increases there is a chance of outage of postgres database. In order to address this we would keep only the recent data in database and provide a query back mechanism to read back from the blockchain for any of the purged data.

Implementation

Based on BLOCKCOUNT
Based on TIME
We can set the purgeMode attribute in config.json file and according to the purge mode, it enables purging from database.
If it is based on blockcount (mention the number of blocks as blockCount value in config.json) ,it will retain those many blocks in the database and the rest of the records would be purged.
If it is based on time (mention the number of days as daysToPurge value in config.json) then it will keep those many days of records in the database according to the daystoPurge provided in the config file.
If the purgeMode attribute is set to "NONE", then purging won't happen and it will retain the complete data as of ledger.

All the audit records of deletion is saved to explorer_audit_table which is further used for the sync process.

Why is this needed?
Explorer creates duplicate copy of complete ledger data in postgres which can be of larger number and can lead to database storage outage.

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #332 

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
```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 12:29:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    added Prometheus metrics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">feature</span>
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
This PR has changes to add support for prometheus metrics.

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

This PR will expose following metrics
-->
```docs
metric_ledger_height
metric_channel_height
metric_channel_transaction_count
metric_node_up
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 06:50:24 +0000 UTC
    </div>
</div>

