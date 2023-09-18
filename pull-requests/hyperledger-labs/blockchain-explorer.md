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
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/454" class=".btn">#454</a>
            </td>
            <td>
                <b>
                    Update Maintainers
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
Update Maintainers - Add Manish and Udhaya
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
        Created At 2023-09-18 05:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/453" class=".btn">#453</a>
            </td>
            <td>
                <b>
                    UI - Fetch Latest Block Time to get channels updation time
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
This feature will display channels updation time, as tooltip, upon hovering on the options from channels dropdown, in header.
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #452 

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
        Created At 2023-09-18 05:36:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/451" class=".btn">#451</a>
            </td>
            <td>
                <b>
                    fix: Catch error when _lifecycle chaincode is not running preventing Synchronizer to shutdown
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

Right now when you set up an empty network that just contains a peer and an orderer and you install an explorer on it it will crash the Synchronizer because it cannot find any chaincodes. 

If it doesn't find any chaincodes it will fallback to the `_lifecycle` chaincode and if that is not installed it will crash because the peer will answer with `Peer XXXXX is not running chaincode _lifecycle`. If then later on blocks are being added or chaincode is installed it won't pick this up.

This is the error that it throws

```
2023-09-11T15:39:05.991Z - error: [SingleQueryHandler]: evaluate: message=Query failed. Errors: ["Error: Peer fab2p1-3041 is not running chaincode _lifecycle"], stack=FabricError: Query failed. Errors: ["Error: Peer fab2p1-3041 is not running chaincode │
│     at SingleQueryHandler.evaluate (/opt/explorer/node_modules/fabric-network/lib/impl/query/singlequeryhandler.js:66:23)                                                                                                                                    │
│     at processTicksAndRejections (internal/process/task_queues.js:97:5)                                                                                                                                                                                      │
│     at async Transaction.evaluate (/opt/explorer/node_modules/fabric-network/lib/transaction.js:319:25), name=FabricError                                                                                                                                    │
│ [2023-09-11T15:39:05.992] [ERROR] Sync - <<<<<<<<<<<<<<<<<<<<<<<<<< Synchronizer Error >>>>>>>>>>>>>>>>>>>>>                                                                                                                                                 │
│ [2023-09-11T15:39:05.992] [ERROR] Sync - Error [FabricError]: Query failed. Errors: ["Error: Peer fab2p1-3041 is not running chaincode _lifecycle"]                                                                                                          │
│     at SingleQueryHandler.evaluate (/opt/explorer/node_modules/fabric-network/lib/impl/query/singlequeryhandler.js:66:23)                                                                                                                                    │
│     at processTicksAndRejections (internal/process/task_queues.js:97:5)                                                                                                                                                                                      │
│     at async Transaction.evaluate (/opt/explorer/node_modules/fabric-network/lib/transaction.js:319:25)                                                                                                                                                      │
│ [2023-09-11T15:39:05.992] [INFO] Sync - <<<<<<<<<<<<<<<<<<<<<<<<<< Closing client processor >>>>>>>>>>>>>>>>>>>>> 
```

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
        Created At 2023-09-12 13:26:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/449" class=".btn">#449</a>
            </td>
            <td>
                <b>
                    BE-447 | fetch latest block time to get channels updation time[backend]
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
To achieve channels updation time on page load, the latest block time needs to be fetched to determine how long ago the channels were updated.

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #447 

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
        Created At 2023-09-12 12:42:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/448" class=".btn">#448</a>
            </td>
            <td>
                <b>
                    feat: Allow explorer to be hosted in a subdirectory
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

Currently the Hyperledger explorer can only be hosted at the root of a domain name. With this change it's possible to also host it at a subdirectory of a domain for example: `https://example.com/your-fabric-explorer-instance`. 

In order to allow this i added the "homepage" property to the package.json as is described in the [create-react-app documentation](https://create-react-app.dev/docs/deployment/#building-for-relative-paths). By using "." for the homepage you it will always fetch the static files relative too where the explorer is being hosted, this way you don't need to change anything at build time. 

Next to that i also changed the location of the api operations to use relative urls as well. This works since a hash-based routing is currently being used.

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
        Created At 2023-09-12 12:41:44 +0000 UTC
    </div>
</div>

