---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7186" class=".btn">#7186</a>
            </td>
            <td>
                <b>
                    In enterprise profile, use sync-mode=FULL and data-storage-format=FOREST
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Also remove lower casing of profile names to keep CLI string values consistent with other options

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-06 13:12:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7181" class=".btn">#7181</a>
            </td>
            <td>
                <b>
                    Enable --Xbonsai-limit-trie-logs-enabled by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Enable `--Xbonsai-limit-trie-logs-enabled` by default, unless sync-mode=FULL.
More info: https://wiki.hyperledger.org/display/BESU/Limit+Trie+Logs+for+Bonsai

When sync-mode=FULL and data-storage-format=BONSAI you get a config validation error at startup...
```
besu --sync-mode=FULL --data-storage-format=BONSAI
2024-06-06 17:36:12.806+01:00 | main | INFO  | Besu | Starting Besu
2024-06-06 17:36:13.027+01:00 | main | ERROR | Besu | Failed to start Besu
...
Cannot enable --Xbonsai-limit-trie-logs-enabled with sync mode FULL
```

I will promote to a Stable option in a separate PR.

This option has been tested on our canaries and by the community since https://github.com/hyperledger/besu/releases/tag/24.3.0

Added a fallback value for the option otherwise specifying --Xbonsai-limit-trie-logs-enabled on the command line, without a value, toggles it back off again.

The `minimalist-profile` has been updated from `bonsai-historical-block-limit=128` to `bonsai-historical-block-limit=512` to avoid further code changes and because I believe there is only a ~60MB difference so using 128 has limited value, see https://github.com/hyperledger/besu/issues/6560#issuecomment-1953928253

I will conservatively set `Xbonsai-limit-trie-logs-enabled=false` in the `enterprise` profile for now as not sure it is desirable.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes https://github.com/hyperledger/besu/pull/6560

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 16:54:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7180" class=".btn">#7180</a>
            </td>
            <td>
                <b>
                    Reduce lock contention on transaction pool when building a block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Currently when Besu builds a block it takes and keep the lock on txpool, until the selection of txs to include is over (and this could be longer of the block creation timeout, since the tx that is processing across the timeout need to complete before releasing the lock) and that could delay the start of the next block building in case of small networks where single nodes could build many blocks in a row, for example L2 sequencers, but the optimization also benefit normal use cases, since incoming txs can be processed and added to the txpool concurrently to a block creation task.

Below there are 2 profiling taken, from a sequencer continuously building blocks,  before and after applying this PR, selected is the layered txpool, and you can see how the 
**Total Blocked Time** went down from >10min to millis.


### Before 

![Screenshot 2024-06-07 114842](https://github.com/hyperledger/besu/assets/91944855/cdd6a21f-94e5-4ab4-94e3-ced8bec66f58)

### After

![image](https://github.com/hyperledger/besu/assets/91944855/4932dcc7-9e4f-4b6a-abf7-f24279b8e8d9)


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-05 13:13:08 +0000 UTC
    </div>
</div>

