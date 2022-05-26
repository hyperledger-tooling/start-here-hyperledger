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
                PR <a href="https://github.com/hyperledger/fabric/pull/3450" class=".btn">#3450</a>
            </td>
            <td>
                <b>
                    Add -buildvcs=false for building binaries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go 1.18 tries to pull git version control information into the binaries that it builds,
based on the presence of .git directory. 'git' is not available when building
the Fabric docker images however, and therefore the build fails.

This change adds -buildvcs=false to the builds to suppress the Go 1.18 behavior change.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 22:07:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3449" class=".btn">#3449</a>
            </td>
            <td>
                <b>
                    Improved gateway error for transient data failure (backport #3445)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3445 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 18:43:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3448" class=".btn">#3448</a>
            </td>
            <td>
                <b>
                    Support PurgePrivateData from the Chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - added handler support for the purgePrivateData
- empty message added to the TxSimulator

DRAFT PR

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
        Created At 2022-05-25 13:35:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3447" class=".btn">#3447</a>
            </td>
            <td>
                <b>
                    Use any peer to evaluate system chaincode transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of d0e209309ce412a66b7a20a6348327f1b2f6ee23 from main branch.

System chaincodes are not included in the installed chaincodes returned by service discovery. The Gateway service was relying on discovery results to find peers on which to evaluate transactions and so failed to evaluate system chaincode transaction functions. Now the Gateway service uses any network peer to evaluate transactions invoked on known built-in system chaincodes.

Also added a system test to confirm that the Gateway service can endorse system chaincode transaction functions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-25 10:10:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3446" class=".btn">#3446</a>
            </td>
            <td>
                <b>
                    Use any peer to evaluate system chaincode transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                System chaincodes are not included in the installed chaincodes returned by service discovery. The Gateway service was relying on discovery results to find peers on which to evaluate transactions and so failed to evaluate system chaincode transaction functions. Now the Gateway service uses any network peer to evaluate transactions invoked on known built-in system chaincodes.

Also added a system test to confirm that the Gateway service can endorse system chaincode transaction functions.

Closes hyperledger/fabric-gateway#434
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 16:23:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3445" class=".btn">#3445</a>
            </td>
            <td>
                <b>
                    Improved gateway error for transient data failure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When transient data is passed to the gateway in a transaction submit, the gateway is more cautious about which orgs it will select to endorse.  It alters the ChaincodeInterest to only allow orgs that are in the distribution policy for the PDCs written to by the chaincode.
This commit doesn’t change the behaviour, but gives a more helpful error message if this layer of protection caused the submit to fail due to the lack of endorsing orgs.
This will help to diagnose issues such as #3328 which took a long time to resolve because of the generic error message.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 14:44:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3442" class=".btn">#3442</a>
            </td>
            <td>
                <b>
                    Fix some errors in the tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

This patch is a solution for errors that occur in the tutorial "Using CouchDB".
First, we added environment variables as in the other tutorials.
Second, we added information to authenticate when using CouchDB.

Signed-off-by: Satoshi Ito <satoshi.ito.tf@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 00:40:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3441" class=".btn">#3441</a>
            </td>
            <td>
                <b>
                    Improve response mismatch logging (backport #3431)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3431 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 12:18:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3440" class=".btn">#3440</a>
            </td>
            <td>
                <b>
                    Log proposal response differences (backport #3420)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Cherry-pick of #3420

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 09:29:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3439" class=".btn">#3439</a>
            </td>
            <td>
                <b>
                    Delete historical versions of private data marked for purging (#3024)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- New feature

#### Description
This PR includes
  - Code for processing the purge marker in the background that deletes
  the historical versions of the private data and corresponding
  hashed-indexed-keys that qualifies for deletion
  - Modifies the transaction number match in the previously committed
   code for filtering the 'to be purged' data so as to have the same
   behavior as for the actually purged data.

#### Related issues
Closes #3024 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 03:51:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3437" class=".btn">#3437</a>
            </td>
            <td>
                <b>
                    bump Go to 1.18.2 (release-2.2) 3 of 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix code issues from the updated staticcheck.
Fix unit test for new TLS messages and assertion changes in Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 21:38:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3436" class=".btn">#3436</a>
            </td>
            <td>
                <b>
                    bump golang.org/x/crypto and golang.org/x/tools (release-2.2) 2 of 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump dependencies in preparation for Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 21:25:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3435" class=".btn">#3435</a>
            </td>
            <td>
                <b>
                    bump go-dockerclient (release-2.2) 1 of 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #2338 in preparation of Go 1.18 update.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 20:56:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3433" class=".btn">#3433</a>
            </td>
            <td>
                <b>
                    [Doc] Remove text for a broken link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

Remove text and broken link


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 08:16:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3432" class=".btn">#3432</a>
            </td>
            <td>
                <b>
                    Remove duplicated line
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 06:50:30 +0000 UTC
    </div>
</div>

