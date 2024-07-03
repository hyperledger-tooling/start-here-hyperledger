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
                PR <a href="https://github.com/hyperledger/besu/pull/7292" class=".btn">#7292</a>
            </td>
            <td>
                <b>
                    --profile to load external profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add support to load external profiles using `--profile` option. The external profiles are expected to be placed in `profiles` directory under besu home (similar to `plugins` directory). This can be overridden using system property `besu.profiles.dir`. Running `./besu --help` should report internal profiles along with external profiles - file names without .toml extension.

External profiles can be used to create custom Besu bundles with various plugins and their default options.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#7265 

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [x] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 10:30:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7291" class=".btn">#7291</a>
            </td>
            <td>
                <b>
                    Turn off CicleCI for Besu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
All the CI jobs run in GitHub actions and Circle CI it no longer needed in Besu project

## Fixed Issue(s)
closes #7283 


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [x] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-03 01:17:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7285" class=".btn">#7285</a>
            </td>
            <td>
                <b>
                    Add next release version after 24.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add next release to the changelog, this commit serves as a bookend for 24.7.0 release

See the latest [release process](https://wiki.hyperledger.org/display/BESU/Release+Process) for more detail 

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
        Created At 2024-07-01 22:41:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7284" class=".btn">#7284</a>
            </td>
            <td>
                <b>
                    Deeper tracing of self-destructed accounts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Consider previously self-destructed accounts when creating accounts.

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
        Created At 2024-07-01 21:37:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7282" class=".btn">#7282</a>
            </td>
            <td>
                <b>
                    Make snap tasks switching
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Convert snap tasks from retrying (same peer) to retrying switching (different peer per retry).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-30 06:28:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7281" class=".btn">#7281</a>
            </td>
            <td>
                <b>
                    Update EIP-2935 contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Use the updated contract and address for EIP-2539.

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
        Created At 2024-06-28 22:18:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7280" class=".btn">#7280</a>
            </td>
            <td>
                <b>
                    Rename ValidatorPublicKey to ValidatorPubKey
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adapt to EIP-7002 name change for validator public key in all places.

## PR description

## Fixed Issue(s)
Besu fix for ethereum/execution-apis#549

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
        Created At 2024-06-28 17:43:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7279" class=".btn">#7279</a>
            </td>
            <td>
                <b>
                    Update limit trie logs validation message for sync-mode=FULL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                > Cannot enable --bonsai-limit-trie-logs-enabled with sync-mode FULL. You must set --bonsai-limit-trie-logs-enabled=false or use a different sync-mode


```
besu --sync-mode=full

BUILD SUCCESSFUL in 14s
95 actionable tasks: 49 executed, 46 up-to-date
2024-06-28 16:24:41.772+10:00 | main | INFO  | Besu | Starting Besu
2024-06-28 16:24:42.441+10:00 | main | ERROR | Besu | Failed to start Besu
picocli.CommandLine$ParameterException: Cannot enable --bonsai-limit-trie-logs-enabled with sync-mode FULL. You must set --bonsai-limit-trie-logs-enabled=false or use a different sync-mode
	at org.hyperledger.besu.cli.options.stable.DataStorageOptions.validate(DataStorageOptions.java:149)
	at org.hyperledger.besu.cli.BesuCommand.validateDataStorageOptions(BesuCommand.java:1579)
	at org.hyperledger.besu.cli.BesuCommand.validateOptions(BesuCommand.java:1546)
	at org.hyperledger.besu.cli.BesuCommand.run(BesuCommand.java:1166)
	at picocli.CommandLine.executeUserObject(CommandLine.java:2026)
	at picocli.CommandLine.access$1500(CommandLine.java:148)
	at picocli.CommandLine$RunLast.executeUserObjectOfLastSubcommandWithSameParent(CommandLine.java:2461)
	at picocli.CommandLine$RunLast.handle(CommandLine.java:2453)
	at picocli.CommandLine$RunLast.handle(CommandLine.java:2415)
	at picocli.CommandLine$AbstractParseResultHandler.execute(CommandLine.java:2273)
	at picocli.CommandLine$RunLast.execute(CommandLine.java:2417)
	at picocli.CommandLine.execute(CommandLine.java:2170)
	at org.hyperledger.besu.cli.BesuCommand.lambda$createExecuteTask$1(BesuCommand.java:1099)
	at picocli.CommandLine.execute(CommandLine.java:2170)
	at org.hyperledger.besu.cli.BesuCommand.lambda$createPluginRegistrationTask$2(BesuCommand.java:1109)
	at picocli.CommandLine.execute(CommandLine.java:2170)
	at org.hyperledger.besu.cli.util.ConfigDefaultValueProviderStrategy.execute(ConfigDefaultValueProviderStrategy.java:58)
	at picocli.CommandLine.execute(CommandLine.java:2170)
	at org.hyperledger.besu.cli.BesuCommand.executeCommandLine(BesuCommand.java:1136)
	at org.hyperledger.besu.cli.BesuCommand.parse(BesuCommand.java:1078)
	at org.hyperledger.besu.Besu.main(Besu.java:41)
Cannot enable --bonsai-limit-trie-logs-enabled with sync-mode FULL. You must set --bonsai-limit-trie-logs-enabled=false or use a different sync-mode
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 06:31:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7278" class=".btn">#7278</a>
            </td>
            <td>
                <b>
                    Promote storage x-trie-log subcommand to trie-log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following https://github.com/hyperledger/besu/pull/7193

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 05:47:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7277" class=".btn">#7277</a>
            </td>
            <td>
                <b>
                    javadoc - Add missing javadoc for evmtool module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
javadoc - Add missing javadoc for evmtool module
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [x] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 02:09:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7275" class=".btn">#7275</a>
            </td>
            <td>
                <b>
                    T8n support for isStateTest and empty accounts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Update t8n executor to support new isStateTest env flag that will
disable extra-transactional processing such as block rewards and beacon
root. Also, make sure such extra-transactional commits don't create 
empty accounts.

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
        Created At 2024-06-27 23:24:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7274" class=".btn">#7274</a>
            </td>
            <td>
                <b>
                    Evm tool readme update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates README for new users
Removes Graal vm use
Corrects JVM install for docker image
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 18:10:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7272" class=".btn">#7272</a>
            </td>
            <td>
                <b>
                    Fix javadoc for ethereum api module, graphql package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix javadoc for ethereum api module, graphql package

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [x] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 12:27:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7271" class=".btn">#7271</a>
            </td>
            <td>
                <b>
                    Add info-level diagnostic logs to aid with resolving stalled BFT chains
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds `INFO` level diagnostic logs to BFT nodes if (and only if) the round for a given block reaches 2 or higher:

```
2024-06-27 10:38:22.076+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:38:22.076+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 4 (Local node)
2024-06-27 10:38:22.077+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 4 

```

It also logs an `INFO` message when the local node expires a round, clearly indicating when the next round will expire, again only if the node reaches round 2 or higher:

```
2024-06-27 10:37:50.011+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundTimer | QBFT round 2 expired. Moved to round 3 which will expire in 32 seconds
```

## Detail

When a BFT chain stalls, the logs are very quiet. Below is an example of a 4-validator chain where 2 validators go offline for 2 minutes and then come back online (note the 4-minute absence of any logs in between blocks `31` and `32`):

```
2024-06-27 10:49:23.015+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Imported #29 / 0 tx / 0 pending / 0 (0.0%) gas / (0xabf6dbf576bfe4f82f51952dbc8cac4e4fc49bc572abe8435e5620825f05498a)
2024-06-27 10:49:24.012+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Produced #30 / 0 tx / 0 pending / 0 (0.0%) gas / (0xbc839f21f03a16e0b686bd6eb2c61ccc4332ee0e53f25503f0df352d87da21a8)
2024-06-27 10:49:25.014+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Imported #31 / 0 tx / 0 pending / 0 (0.0%) gas / (0x6aa4b6a5353857a0691f3014b0d7b4380c5f1fed9d14eb4ee8856d38099ecbb3)
2024-06-27 10:53:25.916+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftRound | Importing proposed block to chain. round=ConsensusRoundIdentifier{Sequence=32, Round=5}, hash=0x6b26c5824251bcdba6df989ed573c9ca73a9c64c0b66720ae1841258c9f2f4c4
2024-06-27 10:53:25.925+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Imported #32 / 0 tx / 0 pending / 0 (0.0%) gas / (0x6b26c5824251bcdba6df989ed573c9ca73a9c64c0b66720ae1841258c9f2f4c4)
2024-06-27 10:53:25.960+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Imported #33 / 0 tx / 0 pending / 0 (0.0%) gas / (0xd9c68d80175333998e7ce391373a2d7098e4be384efd6c9fe9047d3febe6fd43)
2024-06-27 10:53:27.040+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Produced #34 / 0 tx / 0 pending / 0 (0.0%) gas / (0x33e636c3674fe2c2377a422a9f759ce8a162e29ea3385b9c02ea79054eedf908)
```

When this happens it is often necessary to look at `DEBUG` or `TRACE` logs, sometimes on several of the nodes, to determine which round each node has reached and understand if/when the chain will begin producing new blocks.

Reviewers may be concerned about the use of `INFO` logs for these diagnostic messages. My contention is that it is probably reasonable to use `INFO` messages in this case for 3 reasons:

1. As shown in the example above the `INFO` logs are extremely quiet in a stalled-chain case. Giving a summary of where the round-changes are without needing to enable `DEBUG` or `TRACE` is a very useful indicator of whether the user needs to investigate further (e.g. if round changes aren't being received from other nodes) or whether the chain is just waiting for `quorum` nodes to reach the same round. In the cases where blocks are being produced successfully, _**none**_ of the extra log messages are produced.
2. If a BFT chain stalls arguably the only thing the user is interested in is why, and when blocks will start being produced again. So the noise of the extra `INFO` logs in this case isn't obfuscating any other `INFO` logs.
3. The "noisyness" of the logs implicitly reduces over time as the time between round changes increases exponentially

Below is an example of the same 4-validator chain during the same 2-minute stall. Note how once the chain begins producing blocks the new diagnostic messages cease to be written:

```
2024-06-27 10:37:20.025+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Imported #17 / 0 tx / 0 pending / 0 (0.0%) gas / (0x75cbea215b6191af7f997add7c559c17dbc8115f2cd2d9d0c4a15d7f8339363f)
2024-06-27 10:37:21.021+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Produced #18 / 0 tx / 0 pending / 0 (0.0%) gas / (0xf6cb7b1401052466b3e4bc3616600e81f3ddc5f58e8e659674cfb247e9bde2b0)
2024-06-27 10:37:34.005+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundTimer | QBFT round 1 expired. Moved to round 2 which will expire in 16 seconds
2024-06-27 10:37:34.009+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:37:34.009+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 2 (Local node)
2024-06-27 10:37:34.010+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 2 
2024-06-27 10:37:50.011+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundTimer | QBFT round 2 expired. Moved to round 3 which will expire in 32 seconds
2024-06-27 10:37:50.015+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:37:50.015+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 3 (Local node)
2024-06-27 10:37:50.015+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 3 
2024-06-27 10:38:22.014+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundTimer | QBFT round 3 expired. Moved to round 4 which will expire in 64 seconds
2024-06-27 10:38:22.076+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:38:22.076+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 4 (Local node)
2024-06-27 10:38:22.077+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 4 
2024-06-27 10:39:26.017+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundTimer | QBFT round 4 expired. Moved to round 5 which will expire in 128 seconds
2024-06-27 10:39:26.035+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:39:26.035+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:39:26.036+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:40:05.200+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:40:05.202+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:40:05.202+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:40:05.202+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 1 
2024-06-27 10:40:05.215+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:40:05.215+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 1 
2024-06-27 10:40:05.215+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:40:05.216+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:40:05.216+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 1 
2024-06-27 10:40:13.205+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:40:13.205+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 1 
2024-06-27 10:40:13.205+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:40:13.205+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:40:13.205+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 2 
2024-06-27 10:40:13.216+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:40:13.216+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 2 
2024-06-27 10:40:13.216+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:40:13.216+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:40:13.217+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 2 
2024-06-27 10:40:29.211+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:40:29.212+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 2 
2024-06-27 10:40:29.212+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:40:29.212+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:40:29.212+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 3 
2024-06-27 10:40:29.220+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:40:29.221+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 3 
2024-06-27 10:40:29.221+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:40:29.221+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:40:29.221+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 3 
2024-06-27 10:41:01.208+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:41:01.208+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 3 
2024-06-27 10:41:01.208+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:41:01.209+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:41:01.209+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 4 
2024-06-27 10:41:01.223+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:41:01.223+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 4 
2024-06-27 10:41:01.223+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 5 (Local node)
2024-06-27 10:41:01.223+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 5 
2024-06-27 10:41:01.223+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 4 
2024-06-27 10:41:34.021+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundTimer | QBFT round 5 expired. Moved to round 6 which will expire in 256 seconds
2024-06-27 10:41:34.052+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:41:34.052+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 4 
2024-06-27 10:41:34.052+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 6 (Local node)
2024-06-27 10:41:34.052+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 6 
2024-06-27 10:41:34.052+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 4 
2024-06-27 10:42:05.216+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:42:05.217+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 4 
2024-06-27 10:42:05.217+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 6 (Local node)
2024-06-27 10:42:05.217+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 6 
2024-06-27 10:42:05.217+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 5 
2024-06-27 10:42:05.227+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:42:05.227+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 5 
2024-06-27 10:42:05.228+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 6 (Local node)
2024-06-27 10:42:05.228+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 6 
2024-06-27 10:42:05.228+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 5 
2024-06-27 10:44:13.225+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:44:13.227+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 5 
2024-06-27 10:44:13.227+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 6 (Local node)
2024-06-27 10:44:13.227+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 6 
2024-06-27 10:44:13.227+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 6 
2024-06-27 10:44:13.236+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | BFT round summary (quorum = 3)
2024-06-27 10:44:13.236+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xf4ffcf181a94328e848a9622d2d668d9a7035089  Round: 6 
2024-06-27 10:44:13.236+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0xa0685b78b74b63841651855f23d8161482e3bd1b  Round: 6 (Local node)
2024-06-27 10:44:13.236+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x6a5d767a9cfd5711bffefa121491fe9d78d27a27  Round: 6 
2024-06-27 10:44:13.236+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | RoundChangeManager | Address: 0x33b38bbb139832055630194c0673a43b6075663f  Round: 6 
2024-06-27 10:44:13.254+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftRound | Importing proposed block to chain. round=ConsensusRoundIdentifier{Sequence=19, Round=6}, hash=0xa6dcffdd0206a3e0d5dd71bae3ddb67d7905ce0b97e5493ef184f50791f0bbd8
2024-06-27 10:44:13.269+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Imported #19 / 0 tx / 0 pending / 0 (0.0%) gas / (0xa6dcffdd0206a3e0d5dd71bae3ddb67d7905ce0b97e5493ef184f50791f0bbd8)
2024-06-27 10:44:14.026+01:00 | BftProcessorExecutor-QBFT-0 | INFO  | QbftBesuControllerBuilder | Produced #20 / 0 tx / 0 pending / 0 (0.0%) gas / (0x66a847ebf58829312b342764de0fb3b7b656532010b205096985216ee74a2cc5)
```

I did consider concatenating the summary list into a single line, and I accept that reviewers might prefer the PR to use that approach instead of the multi-line logs I've gone with. I tend to prefer logs that are easy for the user to consume by eye and I think the example above shows how easy it is to scan the current round-change status and determine if they need to do any more investigation. But I welcome any comments on the format/verbosity.

- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 09:23:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7270" class=".btn">#7270</a>
            </td>
            <td>
                <b>
                    Fix javadoc for ethereum:core top level package
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix javadoc for ethereum:core top level package

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [x] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 03:32:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7269" class=".btn">#7269</a>
            </td>
            <td>
                <b>
                    javadoc: Adding javadoc for ethstats module
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
javadoc: Adding javadoc for ethstats module. Enabled javadoc lint check for ethstats package

`./gradlew :ethereum:ethstats:javadoc` should not return any errors.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [x] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 02:28:47 +0000 UTC
    </div>
</div>

