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
                PR <a href="https://github.com/hyperledger/iroha/pull/2258" class=".btn">#2258</a>
            </td>
            <td>
                <b>
                    [feature] #2132: Add `endpointN` proc macro
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ilia Churin <churin.ilya@gmail.com>

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
Replaced the declarative macro generating `endpointN` functions with a procedural one in a separate crate.

### Issue
Resolves #2132.
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
Improved readability and extensibility.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
As the macro expansion uses `WarpResult` wrapper defined in `cli/src/torii/utils.rs`, all the users of macro should reexport that struct as well. Alternatively, the macro implementation could be amended to ditch the use of that altogether.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-24 08:16:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2255" class=".btn">#2255</a>
            </td>
            <td>
                <b>
                    Check new pr, do not merge
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
        Created At 2022-05-23 09:39:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2254" class=".btn">#2254</a>
            </td>
            <td>
                <b>
                    [documentation]: Update information on git hooks
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

Updated the readme in `/hooks` and added a reference to it from the contributing guidelines
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 09:03:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2251" class=".btn">#2251</a>
            </td>
            <td>
                <b>
                    [feature] #1926: Added signal handling and graceful shutdown
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

By the architecture of CLI seems the root task that other tasks depend on is spawning Torii's server so I just added a graceful shutdown for the Torii's server. Also I use [Notify](https://docs.rs/tokio/latest/tokio/sync/struct.Notify.html) primitive to notify that the application has received an OS signal because [oneshot channel](https://docs.rs/tokio/latest/tokio/sync/oneshot/index.html) doesn't support multiple receivers.

### Issue

Resolves #1926

### Benefits

Correct completion of all tasks before closing

### Possible Drawbacks

None

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 08:02:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2248" class=".btn">#2248</a>
            </td>
            <td>
                <b>
                    [fix] #1149: Remove nocheckin code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Sam H. Smith <sam.henning.smith@protonmail.com>

### Description of the Change

Removed some development code I left in by accident.

### Issue

#1149

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-23 07:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2246" class=".btn">#2246</a>
            </td>
            <td>
                <b>
                    [documentation]: Flakyness report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span><span class="chip">Tests</span>
            </td>
            <td>
                Signed-off-by: Aleksandr Petrosyan <a-p-petrosyan@yandex.ru>




### Description of the Change

Updated `flakyness.org` (lightweight markup language rendered by GitHub, which has support for spreadsheets, and execution like an `ipython` notebook). 

### Issue
None

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Data

### Possible Drawbacks

Takes long to gather. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-22 09:11:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2244" class=".btn">#2244</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update Iroha CLI documentation
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

Updated readme: https://github.com/outoftardis/iroha/tree/doc-cli/cli#iroha-cli

### Issue

Partially addresses #2193
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 15:25:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2243" class=".btn">#2243</a>
            </td>
            <td>
                <b>
                    Fix/rdb burrow storage tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Burrow storage tests fixes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 13:07:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2240" class=".btn">#2240</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update README for wasm crate
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

Reviewed readme: https://github.com/outoftardis/iroha/tree/doc-wasm/wasm

### Issue

Partially addresses #2193 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-20 07:36:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2239" class=".btn">#2239</a>
            </td>
            <td>
                <b>
                    [fix] #2232: Make Iroha print meaningful message when genesis has too many isi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">UI</span>
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

* Added error message when can't process genesis transaction
* Logger initialization now starts eralier to be able to capture genesis creating logs

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

* Closes #2232 
* Opens #2238 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now users will get more meaningful message when they have too many instructions inside transactions

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

You can take a big genesis from issue description and run Iroha with it to check this out.

I don't think I can write a test for it. This is UI-specific problem

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 20:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2237" class=".btn">#2237</a>
            </td>
            <td>
                <b>
                    [fix] #2170: Fixes build in docker container on M1 machines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                These changes work fine on my Apple Silicon (M1) machine.

I met this problem and I had to fix it in order to do my task.

The reason for the problem is that the toolchain is incorrect here:
`rustup component add rust-src --toolchain nightly-2022-04-20-x86_64-unknown-linux-gnu`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 18:49:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2236" class=".btn">#2236</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update README for macro crate
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

Updated `macro` readme: https://github.com/outoftardis/iroha/tree/doc-macro/macro#iroha-macros

### Issue

Partially addresses #2193 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 14:09:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2235" class=".btn">#2235</a>
            </td>
            <td>
                <b>
                    [feature] #1413: Add API version endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ilia Churin <churin.ilya@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Added a new endpoint that gives back the current API version as a JSON string. 
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue
Resolves #1413.
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits
As we're about to introduce versioning, this will allow end users to check if their client and our API versions match.
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
Set to grab the version from the genesis block, so the endpoint should be usable at all times when a minimal network is up. `ChainIterator` in `wsv`'s `blocks()` method was mentioning possible deadlock, but it should be safe in this case in all I can tell.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests
Added some documentation describing the change in `api_spec.md`.
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
        Created At 2022-05-19 11:03:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2234" class=".btn">#2234</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update Iroha Client and Iroha CLI Client documentation
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

Updates readmes for:

- Iroha Client: https://github.com/outoftardis/iroha/tree/doc-client/client#iroha-client
- Iroha CLI Client: https://github.com/outoftardis/iroha/tree/doc-client/client_cli#iroha-cli-client

### Issue

Partially addresses #2193 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 09:52:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2230" class=".btn">#2230</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update benchmarks documentation
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

Updated readme in `client/benches/tps`: https://github.com/outoftardis/iroha/tree/doc-tps-bench/client/benches/tps#benchmarks-transactions-per-second-tps

### Issue

Partially addresses #2193 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 07:45:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2229" class=".btn">#2229</a>
            </td>
            <td>
                <b>
                    [refactor]: Move `TriggerSet` to `data_model`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
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

Initially it suppose to close #1889 but in the middle of work it was decided to wait until we get dynamic wasm linking. Dynamic linking is important, cause it will remove `no_std` limitations from `data_model` and `TriggerSet` is not compatible with `no_std`.
So this PR contains only `TriggerSet` moving to `data_model`. It should be useful for the future.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

None

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

* `TriggerSet` now is stored there it should be
* Errors produced by `TriggerSet` make more sense

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

None


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 15:54:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2224" class=".btn">#2224</a>
            </td>
            <td>
                <b>
                    [documentation] #2193: Update Parity Scale Decoder Tool documentation
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

Updated README for Parity Scale Decoder Tool: https://github.com/outoftardis/iroha/tree/doc-psd/tools/parity_scale_decoder#parity-scale-decoder-tool

### Issue

Partially addresses #2193 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 07:23:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2223" class=".btn">#2223</a>
            </td>
            <td>
                <b>
                    [ci] #2222: Split tests by whether it involves coverage or not
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ### Description of the Change
- Split tests into 3 jobs
  - `checks`
    - script checks
    - Wasm build check
  - `tests_with_coverage`
    - unit tests #2222
    - integration tests (in a broad sense; crate/tests/*) except for those to be tested in `integration_tests` job
  - `integration_tests` #1683
    - client/tests/integration
    - core/test_network/tests/integration
    - p2p/tests/integration
- Move from `grcov` to `cargo-llvm-cov`
- Include UI tests to coverage profiling #2148

### Issue
- Closes #1683
- Closes #2148
- Closes #2222
- Opens #2242

### Benefits
- Revival of coverage
- Visible coverage failure
- Accuracy of cover rate by #1683 #2148
- CI optimization by #2222

### Possible Drawbacks
- Appearance of 10% or more regression in coverage due to excluding some integration tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 16:54:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2221" class=".btn">#2221</a>
            </td>
            <td>
                <b>
                    Merge commit
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
        Created At 2022-05-17 13:26:25 +0000 UTC
    </div>
</div>

