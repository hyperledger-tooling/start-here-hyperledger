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
                PR <a href="https://github.com/hyperledger/besu/pull/7293" class=".btn">#7293</a>
            </td>
            <td>
                <b>
                    Add evmtool block-test subcommand
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Add an evmtool subcommand that will run non-hive blockchain tests.

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
        Created At 2024-07-03 20:53:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7292" class=".btn">#7292</a>
            </td>
            <td>
                <b>
                    Enhance --profile to load external profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description
Add support to load external profiles using `--profile` option. The external profiles are expected to be placed in `profiles` directory under besu home (similar to `plugins` directory). This can be overridden using system property `besu.profiles.dir`. Running `./besu --help` should report internal profiles along with external profiles - file names without .toml extension.

External profiles can be used to create custom Besu bundles with various plugins and their default options.

Example setup:
- Create `profiles` directory under besu home
- Create `profiles/custom_profile.toml` with configuration values to override.
- Use `./besu --profile=custom_profile ...` to load the custom profile

Docs link: https://besu.hyperledger.org/public-networks/how-to/use-configuration-file/profile

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

