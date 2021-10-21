---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2990" class=".btn">#2990</a>
            </td>
            <td>
                <b>
                    Possible way of adding external builders
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 14:48:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2989" class=".btn">#2989</a>
            </td>
            <td>
                <b>
                    Fix typo on terminal command 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix
- Documentation update

#### Description

Fix typo on terminal command 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-19 09:15:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2988" class=".btn">#2988</a>
            </td>
            <td>
                <b>
                    Check the package name on core/ledger/kvledger UT (#2987)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Check the package name not local file name including "fabric/"
on core/ledger/kvledger unit test

`core/ledger/kvledger` unit-test has been failed on a directory that not "fabric".

Signed-off-by: Justin Yang <justin.yang@themedium.io>

#### Type of change
- Test update

#### Description
Check the error message without "`fabric/`" in `core/ledger/kvledger/snapshot_test.go`
When you run the unit-test in a directory that is not "`fabric`", that unit-test will fail because of checking the filename starting "`fabric/`".

#### Additional details
* Problem
`core/ledger/kvledger/` unit test fails when running the unit-test in another directory, not `fabric/`

```
--- FAIL: TestGenerateSnapshotErrors (13.43s)
    --- FAIL: TestGenerateSnapshotErrors/block_store_returns_error (1.10s)
        snapshot_test.go:571:
            	Error Trace:	snapshot_test.go:571
            	Error:      	"leveldb: closed\ninternal leveldb error while obtaining db iterator\ngithub.com/hyperledger/fabric/common/ledger/util/leveldbhelper.(*DBHandle).GetIterator\n\t/Users/medium/src/hyperledger/fabrictest/common/ledger/util/leveldbhelper/leveldb_provider.go:262\ngithub.com/hyperledger/fabric/common/ledger/blkstorage.(*blockIndex).exportUniqueTxIDs\n\t/Users/medium/src/hyperledger/fabrictest/common/ledger/blkstorage/blockindex.go:304\ngithub.com/hyperledger/fabric/common/ledger/blkstorage.(*BlockStore).ExportTxIds\n\t/Users/medium/src/hyperledger/fabrictest/common/ledger/blkstorage/blockstore.go:105\ngithub.com/hyperledger/fabric/core/ledger/kvledger.(*kvLedger).generateSnapshot\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/kvledger/snapshot.go:114\ngithub.com/hyperledger/fabric/core/ledger/kvledger.TestGenerateSnapshotErrors.func4\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/kvledger/snapshot_test.go:567\ntesting.tRunner\n\t/usr/local/Cellar/go@1.14/1.14.15/libexec/src/testing/testing.go:1050\nruntime.goexit\n\t/usr/local/Cellar/go@1.14/1.14.15/libexec/src/runtime/asm_amd64.s:1373" does not contain "fabric/common/ledger/blkstorage/blockindex.go"
            	Test:       	TestGenerateSnapshotErrors/block_store_returns_error
    --- FAIL: TestGenerateSnapshotErrors/config_history_mgr_returns_error (1.32s)
        snapshot_test.go:581:
            	Error Trace:	snapshot_test.go:581
            	Error:      	"leveldb: closed\ninternal leveldb error while obtaining db iterator\ngithub.com/hyperledger/fabric/common/ledger/util/leveldbhelper.(*DBHandle).GetIterator\n\t/Users/medium/src/hyperledger/fabrictest/common/ledger/util/leveldbhelper/leveldb_provider.go:262\ngithub.com/hyperledger/fabric/core/ledger/confighistory.(*db).getNamespaceIterator\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/confighistory/db_helper.go:114\ngithub.com/hyperledger/fabric/core/ledger/confighistory.(*Retriever).ExportConfigHistory\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/confighistory/mgr.go:221\ngithub.com/hyperledger/fabric/core/ledger/kvledger.(*kvLedger).generateSnapshot\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/kvledger/snapshot.go:120\ngithub.com/hyperledger/fabric/core/ledger/kvledger.TestGenerateSnapshotErrors.func5\n\t/Users/medium/src/hyperledger/fabrictest/core/ledger/kvledger/snapshot_test.go:577\ntesting.tRunner\n\t/usr/local/Cellar/go@1.14/1.14.15/libexec/src/testing/testing.go:1050\nruntime.goexit\n\t/usr/local/Cellar/go@1.14/1.14.15/libexec/src/runtime/asm_amd64.s:1373" does not contain "fabric/core/ledger/confighistory/mgr.go"
            	Test:       	TestGenerateSnapshotErrors/config_history_mgr_returns_error

(...)

FAIL
coverage: 78.8% of statements
FAIL	github.com/hyperledger/fabric/core/ledger/kvledger	583.226s
```

* Reproduce procedure
1. `$ git clone https://github.com/hyperledger/fabric.git fabrictest` or `$ mv fabric fabrictest`
2. `$ cd fabrictest`
3. `$ make unit-test`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 15:15:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2985" class=".btn">#2985</a>
            </td>
            <td>
                <b>
                    Gateway endorsement retry logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Rather than selecting one layout from the discovery endorsement plan and failing if one of the endorsers fails, this commit attempts to create a set of endorsements by retrying the proposal on other endorser until one of the layouts is satisfied.
Additionally, rather than connect to all peers in a channel once on first usage and then never update that cache, this commit adds support for later additions and removals to/from the cache and closing stale connections to peers.

Resolves #2914 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 15:20:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2982" class=".btn">#2982</a>
            </td>
            <td>
                <b>
                    Extra info in log message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add the transaction ID and the orderer endpoint address to the log message before sending the transaction to the orderer.

Resolves https://github.com/hyperledger/fabric-gateway/issues/250

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-14 07:18:04 +0000 UTC
    </div>
</div>

