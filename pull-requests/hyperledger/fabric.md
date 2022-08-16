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
                PR <a href="https://github.com/hyperledger/fabric/pull/3589" class=".btn">#3589</a>
            </td>
            <td>
                <b>
                    Update protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update dependencies to latest fabric-proto-go for consenter mapping

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 10:37:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3588" class=".btn">#3588</a>
            </td>
            <td>
                <b>
                    Add channel capability for V3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry pick of https://github.com/Fabric-orderer-collaboration/fabric/commit/e3fe50b45277ab5e9bbe4bdcc42ddd39060a28f2

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 16:49:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3587" class=".btn">#3587</a>
            </td>
            <td>
                <b>
                    unittest update, fix unittest failed case for TestEcdsaPublicKey
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Test update

#### Description
modify file: bccsp/sw/ecdsa_test.go
reason: with go version 1.19, `x509.MarshalPKIXPublicKey` -> `marshalPublicKey` -> `elliptic.Marshal` will panic if point not on curve because of function new function `panicIfNotOnCurve(curve, x, y)`

```go
func Marshal(curve Curve, x, y *big.Int) []byte {
	panicIfNotOnCurve(curve, x, y)
        // ...
}
```

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
        Created At 2022-08-11 04:17:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3584" class=".btn">#3584</a>
            </td>
            <td>
                <b>
                    Fix inconsistent state between WAL and saved Snapshot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

<!--- Describe your changes in detail, including motivation. -->

It is a [bug](https://github.com/etcd-io/etcd/issues/10219) on etcd.

When an orderer has not participated in the consensus for some time and crashes during the process of writing the latest snapshot to the file, a panic error occurs after the restart.

This bug has been fixed in [etcd](https://github.com/etcd-io/etcd/pull/10356), but not in fabric.

This PR fixes it into the fabric.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-11 03:15:38 +0000 UTC
    </div>
</div>

