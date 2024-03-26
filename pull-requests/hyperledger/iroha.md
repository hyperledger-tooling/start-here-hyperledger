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
                PR <a href="https://github.com/hyperledger/iroha/pull/4384" class=".btn">#4384</a>
            </td>
            <td>
                <b>
                    [refactor]: remove signatures from blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

* remove signatures from blocks stored on chain
Signatures are transient and only applicable during consensus. Since blocks in a blockchain are tied together via block hashes, keeping block signatures after consensus is not only superfluous but also creates issues when replaying blocks when topology has changed (related to #4145)
* removed `consensus_estimation` from block header - it was unused
* removed `event_recommendations` from block - it was unused

## Future work
* Following this PR, block sync protocol should be modified to prevent syncing with malicious peers. This can be done with not too much overhead

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
        Created At 2024-03-25 07:40:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4382" class=".btn">#4382</a>
            </td>
            <td>
                <b>
                    [feature] #4225: Remove genesis signing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Draft implementation of removing genesis signing, still need to finish removing all the private keys where they're no longer necessary

Added additional option for kagami onto crypto command, now it has both genesis signing and key-pair generation options

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4225 <!-- Replace with an actual number,  -->

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
        Created At 2024-03-25 01:22:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4381" class=".btn">#4381</a>
            </td>
            <td>
                <b>
                    [feature] #4350: Expose event set bitfields in schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

Add a new kind of schema metadata - BitmapMeta - and use it to expose `*EventSet` bitfields in schema

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4350 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->


### Checklist

- [ ] make ci pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-22 11:58:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4379" class=".btn">#4379</a>
            </td>
            <td>
                <b>
                    [refactor] #4075: Move metrics related functionality into MetricsReporter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

- sumergai no longer responsible for handling metrics for torii
- fix bug with not proper view change index in metrics

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4075 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->
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
        Created At 2024-03-21 14:09:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4377" class=".btn">#4377</a>
            </td>
            <td>
                <b>
                    [refactor] #4323: telemetry features, tokio console, logs, and configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">config-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

_This is an improved iteration of https://github.com/hyperledger/iroha/pull/4369_

- Remove `logger.tokio_console_address` configuration parameter entirely: this could be configured in a more refined way using default ENVs (see [`console_subscriber` docs](https://docs.rs/console-subscriber/0.2.0/console_subscriber/struct.Builder.html#method.with_default_env))
- Rename `[telemetry.dev]` config section to `[dev_telemetry]`
- Update `telemetry` and `dev-telemetry` features of `iroha`
- Update `tokio-console` feature of `iroha_logger`: now console seamlessly starts whenever this feature is enabled
- Improve logs & warnings
- Fix dev-telemetry file logs: separate each item with `\n`, and recursively create parent directories
- Improve config validation: handle file paths

### Linked issue

Closes #4323 

### Benefits

- Less config parameters
- More flexible way to configure tokio console
- Less feature mess (?)
- Better warnings
- Refactoring

### Checklist

- [x] Document how to use tokio console
- [x] Figure out what happened to `Cargo.toml`s
- [x] Check manually several cases, how Iroha behaves with `telemetry`/`dev-telemetry` features enabled depending on `telemetry` configuration (warnings, logs, file output)
- [x] Check manually Tokio Console (works, but requires `TRACE` log level)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-21 02:00:35 +0000 UTC
    </div>
</div>

