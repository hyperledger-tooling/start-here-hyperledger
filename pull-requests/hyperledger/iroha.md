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
                PR <a href="https://github.com/hyperledger/iroha/pull/4377" class=".btn">#4377</a>
            </td>
            <td>
                <b>
                    [refactor] #4323: re-arrange telemetry & tokio console config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">config-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

_This is an improved iteration of https://github.com/hyperledger/iroha/pull/4369_

- Remove `logger.tokio_console_address` configuration parameter entirely: this could be configured in a more refined way using default ENVs (see [`console_subscriber` docs](https://docs.rs/console-subscriber/0.2.0/console_subscriber/struct.Builder.html#method.with_default_env))
- Update `telemetry` and `dev-telemetry` features of `iroha`
- Update `tokio-console` feature of `iroha_logger`: now console seamlessly starts whenever this feature is enabled
- Improve warnings

### Linked issue

Closes #4323 

### Benefits

- Less config parameters
- More flexible way to configure tokio console
- Less feature mess (?)
- Better warnings

### Checklist

- [ ] Document somewhere how to use Tokio Console?
- [ ] Figure out what happened to `Cargo.toml`s

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-21 02:00:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4375" class=".btn">#4375</a>
            </td>
            <td>
                <b>
                    [refactor] #4259: Make Action and Filter non-generic types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Make the `Action` and `Filter` types exported from `iroha_data_model` non-generic. This is used by code in `iroha_core`, so make generic copies in there. There's no need to complicate the public API due to the requirements of the implementation.

This also makes the `Action` constructor accept `impl Into<TriggeringEventFilterBox>` as a filter, simplifying most API invocations. Additional shorthand conversions from concrete event filter types are added (for example `AccountEventFilter -> TriggeringEventFilterBox`) to reduce the required boilerplate even more.

### Linked issue

Closes #4259

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

No unnecessary generic in the API -> better code completion and easier API.

### Checklist

- [ ] make CI pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-19 10:18:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4374" class=".btn">#4374</a>
            </td>
            <td>
                <b>
                    [fix] #0000: Disable snapshot read/write in tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

When running tests in parallel, they race for the same snapshot file.
Since persistency isn't required in tests it's better to disable snapshot in tests.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 09:51:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4371" class=".btn">#4371</a>
            </td>
            <td>
                <b>
                    [poc] DO NOT MERGE: shared account ID is off curve
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

- Proof of concept for the new account, with non-essential parts omitted
  - There is room for optimization in actual implementation
- This is in the form of a draft PR just for review and not expected to be merged

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- The concept demonstrated here is https://github.com/hyperledger/iroha/issues/2085#issuecomment-1985152267
- Intended to be one of the foundations for #2083 in general and #4373 in particular

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-18 07:33:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4370" class=".btn">#4370</a>
            </td>
            <td>
                <b>
                    [refactor] #4291: update genesis config & schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">question</span><span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">config-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

- remove inline executor mode
- rename field to `executor_file`
- remove genesis from schema (revert #1391).
  - **Why?**
  - Because it doesn't belong here. It's not a part of the data model, but rather of the configuration system. The original reasoning about "ease for SDK developers" doesn't work (genesis is JSON, but schema is about SCALE; types are straightforward).

### Linked issue

Closes #4291 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 03:20:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4368" class=".btn">#4368</a>
            </td>
            <td>
                <b>
                    [feature] #4285: Verifiable Random Function in Sumeragi
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ## Description
Adds a crypto primitive and randomization of the topology on block commits.

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4285

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 22:35:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4367" class=".btn">#4367</a>
            </td>
            <td>
                <b>
                    [fix] #4292, #4327: Docker follow-up on configuration update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">config-changes</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

- Actualised Dockerfile(s)
- Added actual parsing of `SUMERAGI_TRUSTED_PEERS` env
- Refactor guts of config implementation

### Linked issue

Closes #4292, #4327

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 06:58:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4366" class=".btn">#4366</a>
            </td>
            <td>
                <b>
                    [refactor] #4315: split pipeline events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

* introduced `WithEvents` which makes sure that events are consumed upon block state transition
* refactored `PipelineEvent` to a more sane representation

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 06:47:35 +0000 UTC
    </div>
</div>

