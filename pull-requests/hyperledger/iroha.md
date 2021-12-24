---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1752" class=".btn">#1752</a>
            </td>
            <td>
                <b>
                    [fix] #1751: Sumeragi awaits wsv block commit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Egor Ivkov <e.o.ivkov@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
- Sumeragi awaits wsv block commit
- Update for network topology now directly from sumeragi
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
#1751
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Fixes double spend attack, and general bug with same transaction being committed more than once. For more detailed overview please read the issue.

Previously wsv was updated after kura when it received the message from sumeragi. The bug was in the fact that sumeragi assumed it committed the block and updated its state, therefore able to approve next blocks, but the message might arrive to Kura a lot later. This made possible for the `is_in_blockchain` checks for transactions to pass sometimes even as some of them were in previous block. And therefore leaders could create blocks with same txs and other peers might approve it.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 19:08:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1750" class=".btn">#1750</a>
            </td>
            <td>
                <b>
                    Getting Error code from burrow execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Add possibility to get info why Burrow execution failed, what is stateful validation error code
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Ability to get error code from smart contract execution, know why it failed
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 12:54:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1748" class=".btn">#1748</a>
            </td>
            <td>
                <b>
                    [feature] #1179: Add revoke-permission-or-role instruction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>

[feature] #1179: Add revoke instruction.

Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

- Introduced Revoke isi. 
- Introduced RevokeBox implementations. 
- introduced very basic permissions validators for said Revoke isi. 
- Re-organised the permissions-validators crate 

### Issue

Closes #1179.


<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

- Can revoked granted permissions. 
- permissions validators crate is much easier to navigate. 

### Possible Drawbacks
None

### Usage Examples or Tests *[optional]*
TODO. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-23 07:04:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1746" class=".btn">#1746</a>
            </td>
            <td>
                <b>
                    [fix] #1715: Consensus fixes to handle high load
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

View change handling fixes

- View change proofs made independent of particular transaction hashes
- Reduced message passing
- Collect view change votes instead of sending messages right away (improves network resilience)
- Fully use Actor framework in Sumeragi (schedule messages to self instead of task spawns)

Improves fault injection for tests with Sumeragi

- Brings testing code closer to production code
- Removes overcomplicated wrappers
- Allows Sumeragi use actor Context in test code

Batch transaction gossiping

Significantly reduces message passing

Also fixes transaction count metric calculation, which previously was providing results delayed by 1 block.

### Issue
#1715
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

- Network is more resilient - will recover in cases of faulty peers or after high load (when the load normalizes)
- Network is more performant: about 2 TPS previously, now 100 TPS

For measuring TPS:
- Python script was used
- Timeouts in config were increased
- Logging level was set to `ERROR`
- 4 peers through docker compose were ran locally on a machine with 16 GB or RAM, i7 8th gen.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 09:23:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1745" class=".btn">#1745</a>
            </td>
            <td>
                <b>
                    [fix] #1404: Verify fixed.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Added test to verify that it's possible to both register and mint an asset in one `tx`. 

### Issue

Closes #1404

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

More tests. 

### Possible Drawbacks

More tests. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 09:18:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1744" class=".btn">#1744</a>
            </td>
            <td>
                <b>
                    [fix] #1742: Concrete errors returned in `core` instructions.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Opaque `eyre::Report`s have been replaced with specific `Error` enums. 

### Issue

Closes #1742 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Opaque error types that could only have been printed are now also possible to handle and match. 


### Possible Drawbacks

None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-22 06:06:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1743" class=".btn">#1743</a>
            </td>
            <td>
                <b>
                    [feature] #1734: Validate `Name` to exclude whitespaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change
- Prohibit a whitespace from getting into a `Name` of domain, account, asset, metadata key, and permission token.
- Identify `Domain` by `Id` instead of `Name`

Now `Id::new`s return `Result<Self>`, while previous implementations are left as `Id::test`s for usability

### Issue
Close #1734

### Benefits
Type level guarantee of no whitespaces in `Name` 

### Possible Drawbacks
There might be a better error handling for `Name` validation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-21 15:08:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1741" class=".btn">#1741</a>
            </td>
            <td>
                <b>
                    Docs: Information about swarm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sara <lira.lemur@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Added link to Kuvaldini's swarm tool

### Issue

none

### Benefits

Link to a good tool on deployment (which is extremely difficult atm) 

### Possible Drawbacks


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 13:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1739" class=".btn">#1739</a>
            </td>
            <td>
                <b>
                    [fix] #1636, #1249: Remove `trusted_peers.json` and `structopt`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

- Remove the required command-line flag for specifying the `trusted_peers.json` file. 
- Remove `structopt` from `iroha_core`. 

### Issue

Closes #1636. 
Closes #1249. 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

- Simpler configuration. 
- Structopt wasn't doing much in `iroha_core` beyond making compilation take longer. 

### Possible Drawbacks

Not really a drawback, but If `trusted_peers` is a large `json` array, they still need to be specified in `config.json`. 

### Usage Examples or Tests *[optional]*

by setting the environment variables, anywhere in the iroha git folder. 
```bash
cargo run --bin iroha -- --submit
```
for a short override and same effect, 
```bash
IROHA2_GENESIS_PATH="/home/app/Git/iroha/configs/peer/genesis.json" IROHA2_CONFIG_PATH="/home/app/Git/iroha/configs/peer/config.json" cargo run --bin iroha -- --submit
```

### Alternate Designs *[optional]*

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-19 08:25:59 +0000 UTC
    </div>
</div>

