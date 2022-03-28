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
                PR <a href="https://github.com/hyperledger/iroha/pull/2015" class=".btn">#2015</a>
            </td>
            <td>
                <b>
                    RC3 Release PR
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Notable SDK-related changes

- Schema changes that fix #1969 
- Schema endpoint (use `curl -X GET http://127.0.0.1:8080/schema`)
- WASM decode optimisations
- timed triggers
- Improved API for generating ISI (documentation pending)
- By-call triggers

### Release checklist
- [ ] The crates have been version bumped.
- [ ] Iroha passed
  - [ ] `cargo hack` tests
  - [ ] functional tests 
  - [x] CI tests
- [ ] Iroha lasted for five days at the longevity stand
- [ ] Benchmarks
  - [ ] Rust-based (depends on #1963 @s8sato)
  - [ ] Torii
  - [ ] Load script on real hardware
- [ ] Iroha documentation
  - [x] Readme
  - [ ] api_spec
  - [ ] tutorial
- [ ] SDKs compiled successfully using the schema from latest branch (Hash: 9a149eecb00485f71fd23179dd16a73815d739b2)
  - [ ] Java
  - [ ] JavaScript
  - [ ] Swift
- [ ] All SDK tests pass
  - [ ] Java
  - [ ] JavaScript
  - [ ] Swift
- [ ] (Optional) SDKs implemented the main features added in the current release:
  - [ ] Schema endpoint querying
  - [ ] Timed triggers
  - [ ] Event-based triggers

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 05:51:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2014" class=".btn">#2014</a>
            </td>
            <td>
                <b>
                    [fix] #2013: Hotfix CLI args.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

- Accept empty args which are sometimes passed by `exec`. 
- Fixed CI coverage workflow. 
- Generate changelog for the March Release

### Issue

Closes #2013

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Changelog, working CLI args, working push workflow. 

### Possible Drawbacks

None


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 05:40:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2006" class=".btn">#2006</a>
            </td>
            <td>
                <b>
                    [feature] #1621: Introduce By Call Triggers
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

- Added new `ExecuteTrigger` *ISI*
- Added new event and filter: `ExecuteTriggerEvent` and `ExecuteTriggerEventFilter`
- Changed `WSV` so that every clone stores its own copy of events. No reference counting anymore
- Added some integration tests for a new instruction
- Opened #2005 

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #1621 

<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Now we can execute trigger by ISI call

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

Can't see any

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests

See `client/test/integration/triggers/by_call_trigger.rs`

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 22:54:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/2002" class=".btn">#2002</a>
            </td>
            <td>
                <b>
                    [feature] #1970: Add optional schema endpoint
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

Add optional schema endpoint

### Issue
Closes #1970 


### Benefits

Optional Schema endpoint 

### Possible Drawbacks

Slightly increased binary size.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 08:01:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1999" class=".btn">#1999</a>
            </td>
            <td>
                <b>
                    Fix/main to develop merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description of the Change
Main to develop synchronization.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 07:13:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1993" class=".btn">#1993</a>
            </td>
            <td>
                <b>
                    [ci]: Add telemetry to default features. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru><!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

- Add telemetry to default features as per @Cre-eD 's request. 
- Update outdated `README.md` files. 

### Issue

Closes #1979 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

Default deployment has support for prometheus metrics

### Possible Drawbacks

Increased binary size. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 06:58:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1989" class=".btn">#1989</a>
            </td>
            <td>
                <b>
                    [fix] #1897: Removed usize/isize from serialization
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

In all the locations where a struct derives Serialize or Deserialize usize has been replaced
with either u64 or u32. No instances of isize existed. In the cases where code using the
data required a usize u32 was chosen as the replacement. There is no point in avoiding usize
in the on disk formats if 32-bit platforms can't read and use the values written.

### Issue

Resolves #1897 
<!-- Put in the note about what issue is resolved by this PR, especially if it is a GitHub issue. It should be in the form of "Resolves #N" ("Closes", "Fixes" also work), where N is the number of the issue.
More information about this is available in GitHub documentation: https://docs.github.com/en/github/managing-your-work-on-github/linking-a-pull-request-to-an-issue#linking-a-pull-request-to-an-issue-using-a-keyword -->

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

No chance of crashing due to serializing on 64-bit then deserializing on 32-bit or vice versa.

### Possible Drawbacks

This change limits the size of certain configuration values to 4 billion. Probably a non issue.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 22:30:27 +0000 UTC
    </div>
</div>

