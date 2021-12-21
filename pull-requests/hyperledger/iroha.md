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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1738" class=".btn">#1738</a>
            </td>
            <td>
                <b>
                    [feature] #1144: Add metadata nesting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

- Moved metadata module into its own file. 
- Added a `LimitedMetadata` variant  to `Value`, 
- Adding an `Unlimited` variant can cause problems in preserving code invariants.
- Added the `nested_` family of `fn`s, which all operate on a `&Path`, which is a type alias for `Vec<String>` (for now). 
- Nested get, remove and insert functions fail fast if the path is either empty, incorrect, or malformed. 
- Added tests to verify functionality. 


### Issue

Closes #1144 

### Benefits

Nested metadata. 

### Possible Drawbacks

None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 14:02:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1736" class=".btn">#1736</a>
            </td>
            <td>
                <b>
                    [ci]: Update Mold 1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>


### Description of the Change
Updated to Mold v1.0

### Issue

None

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Production-ready linker

### Possible Drawbacks

None


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 07:33:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1735" class=".btn">#1735</a>
            </td>
            <td>
                <b>
                    Feature/healthcheck
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
Added healthcheck interfaces via:
- http
- grpc
- metrics

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

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
        Created At 2021-12-17 06:03:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1732" class=".btn">#1732</a>
            </td>
            <td>
                <b>
                    [fix] #666: Fixed a problematic typo in previous PR.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Fix Small Typo

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-14 15:26:21 +0000 UTC
    </div>
</div>

