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
                PR <a href="https://github.com/hyperledger/iroha/pull/2209" class=".btn">#2209</a>
            </td>
            <td>
                <b>
                    I2 dco
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
        Created At 2022-05-13 08:58:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2197" class=".btn">#2197</a>
            </td>
            <td>
                <b>
                    [feature] #2100: Add query to find all accounts with asset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
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

* Added `FindAccountsWithAsset` query
* Added test for it
* Fixed bug when block events (including `Committed` event) were sent before actual block applying to *WSV*
* Cause of this bugfix some of previously flaky tests are no longer such. Tested with `cargo flaky` running every test for **100** times for about 4 hours
* Smartcontract test is enabled back as it seems not being flaky anymore. But still takes about 50 secs to complete on my machine

Results of running ```cargo flaky``` (edited for readability):
```
====== FOUND 4 FAILING TESTS ======
- test: two_networks stdout
failures: 1/100 (1%)

- test: integration::unregister_peer::unstable_network_stable_after_add_and_after_remove_peer stdout
failures: 2/100 (2%)

- test: config::tests::parse_example_json stdout
failures: 100/100 (100%)

- test: ui stdout
failures: 600/100 (600%)
```

The **3'rd** case isn't a real problem. This test just depends on a folder it runs from, we should be able to fix it probably.
The **4'th** case is a compilation tests (as @mversic suggested). Not sure what does it means here.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2100 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* New query
* Less number of flaky tests

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

I've enabled `mint_nft_for_every_user_every_1_sec` test back. I haven't run `cargo flaky` with it but I've run it mannually (bash script) for about 30 times and it seems to work fine. The only problem is a long execution time (~50 sec on my M1 Mac), so probably I need to ignore this test again.

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

```bash
cargo test --package iroha_client --test mod -- integration::queries::account::find_accounts_with_asset --exact --nocapture
```

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 20:32:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2196" class=".btn">#2196</a>
            </td>
            <td>
                <b>
                    [documentation] #2119: Add guidance on how to hot reload Iroha in a Docker container
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

Add guidance on how to hot reload Iroha in a Docker container: https://github.com/outoftardis/iroha/blob/doc-hot-reload-guide/docs/source/guides/hot-reload.md

### Issue

Closes #2119 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 15:45:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2195" class=".btn">#2195</a>
            </td>
            <td>
                <b>
                    [documentation] #1280: Document Iroha metrics
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

Add documentation for metrics: https://github.com/outoftardis/iroha/blob/doc-metrics/docs/source/guides/metrics.md

### Issue

Partially addresses #1280 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 14:40:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2194" class=".btn">#2194</a>
            </td>
            <td>
                <b>
                    [feature] #1149: Block amount.
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

Take what was the previous file name, prepend with zeroes, then interpret that as dir + file name. So block files are ex 2/003, 0/032 et cetera.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

#1149 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Most operating systems will freak out if there are too many files in a directory. This solves that.

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

We still iterate over all existing files to figure out which block file we want to edit/create. I think this needs to change in the long run. We should using a simple formula map from block number to block file number. That way you only touch the the file you want to operate on. That is a seperate issue from #1149 though, so the point is irrelevant for this PR.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 12:16:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2190" class=".btn">#2190</a>
            </td>
            <td>
                <b>
                    [documentation] #2181: Review README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

### Description of the Change

Review README. View file: https://github.com/outoftardis/iroha/tree/doc-readme-review#hyperledger-iroha

### Issue

Addresses #2181 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 07:56:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2189" class=".btn">#2189</a>
            </td>
            <td>
                <b>
                    Remove running build from comment
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

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
https://hackerone.com/reports/1548870
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Remove potential injection
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
        Created At 2022-05-11 03:04:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2188" class=".btn">#2188</a>
            </td>
            <td>
                <b>
                    [fix] #1990: Enable peer startup via env vars in the absence of `config.json`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ilia Churin <ilia.ch@netogami.net>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->
In the case when the minimal cli client (`iroha`) was provided with no `config.json` either in the same directory or as an environment variable, do not stop the execution, but instead require that all the variables from the default json be provided as environment variables too, and load them onto default configuration.

### Issue

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->
Resolves #1990.

### Benefits
Presumably easier and more flexible setup of peer through cli.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
As the fix chooses to fall back on default impl for config, it has the same problems that were discussed in #2101 and  #2118. The question is which variables should be allowed to be set via environment, and which subset of them should be required when using default, if we're going to stick with it at all. As of now, the default configuration is generated with `Default` and all the variables from the `configs/peer/config.json` are required to proceed if no file was found.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

<!-- ### Usage Examples or Tests *[optional]* -->

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

<!-- ### Alternate Designs *[optional]* -->

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
        Created At 2022-05-10 09:30:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2187" class=".btn">#2187</a>
            </td>
            <td>
                <b>
                    [fix] #2150: Use `rustfmt` instead of `cargo fmt` in `client/build.rs`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">build</span>
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

`cargo fmt` usage was replaced by `rustfmt` directly. This is a more clean way to avoid cargo recursion problem (instead of just removing `CARGO_RECURSION` env-variable)

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closed #2150 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

More *legal* way to solve cargo recursion problem for formatting smartcontract

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Maybe non-trivial for multi-files smartcontracts

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 19:22:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2185" class=".btn">#2185</a>
            </td>
            <td>
                <b>
                    [feature] #2186: Add transfer instructions for all asset types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
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

- Expose `Mintable` and `MintabilityError` in `prelude`. 
- Replace `#[log]` annotations with explicit trace instructions. 
- Add `Transfer` implementations for `Asset`s of `Fixed` and `u128` types. 
- Refactor `Error` implementations. 
- Refactor `data_model`. 


### Issue

Closes #2149
Closes #2036
Closes #2186 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Smaller code.

### Drawbacks

None. 
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

