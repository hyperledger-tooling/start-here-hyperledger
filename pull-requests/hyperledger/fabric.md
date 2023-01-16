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
                PR <a href="https://github.com/hyperledger/fabric/pull/3931" class=".btn">#3931</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: lifecycle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description
Orderer v3: Remove system channel usage from integration tests: lifecycle

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note

Epic: #3511
Issue: #3515


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 15:22:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3930" class=".btn">#3930</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Orderer v3: Remove system channel usage from integration tests: ledger


#### Related issues

Epic: #3511
Issue: #3515
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 13:27:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3929" class=".btn">#3929</a>
            </td>
            <td>
                <b>
                    Support for Couchdb JWT Authentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added support for couchdb JWT Authentatication via RSA256 algorithm.

Signed-off-by: Aviral Agrawal <aviral.agrawal@dltlabs.io>

#### Type of change

- New feature

#### Description

Added support for token based JWT authentication supported in Couchdb by generating JWT token using RSA256 algorithm. 

#### Related issues

https://github.com/hyperledger/fabric/issues/3317

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 08:03:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3925" class=".btn">#3925</a>
            </td>
            <td>
                <b>
                    Update purge private data integration tests (backport #3813)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3813 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-14 21:02:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3924" class=".btn">#3924</a>
            </td>
            <td>
                <b>
                    Fix bug in purging private key from statedb (backport #3923)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3923 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-14 20:59:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3923" class=".btn">#3923</a>
            </td>
            <td>
                <b>
                    Fix bug in purging private key from statedb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

This PR
- Makes the read of private key via hashed-index from the private data store, prior to adding the purge-marker, so as to avoid the race condition, where the hashed-index entries could be deleted via the background process, before they are read in the commit path.

- Deletes the purged key from statedb even when the private key is overwritten by a succeeding transaction in the block, and the corresponding private data is missing

#### Type of change
- Bug fix

#### Related issues
closes #3828 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-14 04:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3922" class=".btn">#3922</a>
            </td>
            <td>
                <b>
                    synchronize access to wal storage from chain and node (backport #3919)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3919 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-13 23:00:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3920" class=".btn">#3920</a>
            </td>
            <td>
                <b>
                    Fix basic checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A few recent PRs broke basic CI checks, this commits address linter and docs update issues.

Signed-off-by: Artem Barger <artem@bargr.net>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 06:39:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3919" class=".btn">#3919</a>
            </td>
            <td>
                <b>
                    synchronize access to wal storage from chain and node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description
sychronized the access to raft/wal stroage from
node ready loop and chain apply go routine

#### Related issues
#3903 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-12 11:23:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3918" class=".btn">#3918</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: idemix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: Remove system channel usage from integration tests: gossip
#### Related issues

Epic: #3511 
Issue: #3515 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-12 11:07:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3917" class=".btn">#3917</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: gossip
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: Remove system channel usage from integration tests: gossip

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

Epic: #3511 
Issue: #3515 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-12 10:27:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3916" class=".btn">#3916</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: Remove system channel usage from integration tests: gateway

#### Related issues
Epic: #3511
Issue: #3515
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 15:02:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3913" class=".btn">#3913</a>
            </td>
            <td>
                <b>
                    Fail-fast fetching potentially purged data during block commit (backport #3907)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3907 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-11 12:52:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3911" class=".btn">#3911</a>
            </td>
            <td>
                <b>
                    [WIP] Check PurgedKeyAuditLogging messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 18:08:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3910" class=".btn">#3910</a>
            </td>
            <td>
                <b>
                    Update purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Include multiple purge transactions in a single block

Also removes placeholder for seperate test to check data is actually removed from the peer since there is no api available to confirm that- see issue #3844

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 17:08:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3909" class=".btn">#3909</a>
            </td>
            <td>
                <b>
                    Rename ThreeOrgRaft nwo standard networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The name has changed in the main branch as a result of hyperledger#3643 and hyperledger#3853, and this rename should make it easier to backport PRs with mergify

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 11:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3907" class=".btn">#3907</a>
            </td>
            <td>
                <b>
                    Fail-fast fetching potentially purged data during block commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

This PR avoids keep trying behavior for fetching private data during block commit, in a situation where the hashes may not match because the private data may potentially have been purged. Instead, such data is treated as an eligible missing data that the peer would try later in the background reconciliation process.

#### Type of change
- New feature

#### Related issues
[Issue #3858](https://github.com/hyperledger/fabric/issues/3858)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 23:56:22 +0000 UTC
    </div>
</div>

