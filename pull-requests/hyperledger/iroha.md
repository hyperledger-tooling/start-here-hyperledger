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
                PR <a href="https://github.com/hyperledger/iroha/pull/2185" class=".btn">#2185</a>
            </td>
            <td>
                <b>
                    [refactor] #2149: Expose `Mintable` and `MintabilityError` in `prelude`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Small PR to address #2149. 

### Issue

Closes 2149

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Smaller code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 14:06:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2184" class=".btn">#2184</a>
            </td>
            <td>
                <b>
                    [fix] #2159: Improve `parity_scale_decoder` tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">Tests</span>
            </td>
            <td>
                Signed-off-by: Daniil Polyakov <arjentix@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Previously `parity_scale_decoder` tests were using hardcoded string to compare with the result. Now objects are stored instead. It's easier to read and update.

I can't use `serde_json` here (as proposed in the issue), because this program output isn't exactly *json*. It's the output of `Debug` trait which has type name for every field.
 
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2159 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* Easier to read
* Easier to update

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

```bash
cargo test --package parity_scale_decoder --bin parity_scale_decoder -- tests --nocapture
```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs

We can change `parity_scale_decoder` implementation to use `serde::de::Serialize` instead of `Debug`. But I don't think we need it. This approeach will decrease the number of supported types and probably will give less info about a type

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
        Created At 2022-05-06 21:37:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2183" class=".btn">#2183</a>
            </td>
            <td>
                <b>
                    [feature] #1883: Remove embedded configuration files.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

### Description of the Change

Removed sample configurations from the docker file. Adjusted docker compose to work from the root of the repository clone. 

### Issue

Closes #1883 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

No problems with unspecified or incorrectly specified configuraion/genesis. 

### Possible Drawbacks

More involved process of running an iroha peer. 

### Usage Examples or Tests *[optional]*

```
docker compose up
```

Inside existing docker compose fields, please add a line with the following: 

```
volumes: 
 - <path-to-config-and-genesis>:config
```


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 09:19:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2182" class=".btn">#2182</a>
            </td>
            <td>
                <b>
                    Remove launch from comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: safinsaf <safinsaft@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Remove potential injection
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
        Created At 2022-05-06 08:36:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2180" class=".btn">#2180</a>
            </td>
            <td>
                <b>
                    [documentation] #2113: Document features in Cargo.toml files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

### Description of the Change

Provide descriptions of features in `Cargo.toml` files

### Issue

Closes #2113 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 06:10:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2178" class=".btn">#2178</a>
            </td>
            <td>
                <b>
                    [documentation] #2177: Clean up gitchangelog output
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

### Description of the Change

Addressed Aleksandr's input about changelog

- Added the script to remove the names at the end of log messages after the log is built
- Updated gitchangelog config to automatically remove signed-off part of the commit and the PR number.
- Updated gitchangelog to ignore commits about codeowners
- Cleaned up the logs (partially), mainly addressing the issue with nested lists of changes.

[gitchangelog output](https://github.com/outoftardis/iroha/blob/doc-changelog/CHANGELOG.rst)

### Issue

Fixes #2177 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-05 02:53:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2174" class=".btn">#2174</a>
            </td>
            <td>
                <b>
                    [ci]: Version bump all of the crates.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

### Description of the Change
Version bump

### Issue
None

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Version bump

### Possible Drawbacks

None

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-04 06:06:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2173" class=".btn">#2173</a>
            </td>
            <td>
                <b>
                    [feature] #2004: Forbid `isize` and `usize` from becoming `IntoSchema`.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>

### Description of the Change

Add a unit test that fails when `usize`/`isize` are `Encode`/`Decode`/`IntoSchema`

### Issue

Closes #2004 

### Benefits

Impossible to add structures which utilise `usize`, `isize` inside the schema, and thus cause UB in decoding if the pointer size on the host machine is smaller than the encoded integer.

### Possible Drawbacks
None

### Usage Examples or Tests *[optional]*


```
cargo test -p iroha_schema --test architecture-dependent
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 18:49:57 +0000 UTC
    </div>
</div>

