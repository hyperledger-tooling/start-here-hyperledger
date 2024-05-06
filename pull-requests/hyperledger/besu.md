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
                PR <a href="https://github.com/hyperledger/besu/pull/7029" class=".btn">#7029</a>
            </td>
            <td>
                <b>
                    Update license header formatting (HL 4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Apply license header formatting fixes to :plugin-api and :util sub-projects.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785 

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
        Created At 2024-05-02 07:14:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7028" class=".btn">#7028</a>
            </td>
            <td>
                <b>
                    Authcall
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - adds AUTH and AUTHCALL opcodes to Prague evms.
- adds a mutable authorizedBy:Address field to the MessageFrame
- adds AUTH opcode costing to gas calculators
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-01 11:39:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7027" class=".btn">#7027</a>
            </td>
            <td>
                <b>
                    World state halt and chain halt fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Further improvements to fix the world state halts and some cases of the chain halt.

- Added pivot block checks back into the snap sync pipeline to prevent world state halting due to not having the current pivot block. The World State pipeline could halt due to a chain halt since it depended on block added events to check for new pivot blocks.
- Made the pivot block check in the snap worldstate pipeline async and this was called on the block added event from the chain download pipeline and blocked the import thread
- Added time to the pivot block selector and decreased the timeout in the DynamicPivtoBlockSelector from 5 minutes to 20 seconds
- Disconnect peers when we only receive a partial response for block headers after multiple tries. Some nodes were only sending a response of a single header instead so we would get stuck in the chain download.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixed #6908 

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
        Created At 2024-05-01 02:13:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7025" class=".btn">#7025</a>
            </td>
            <td>
                <b>
                    build - Update license headers formatting (HL 3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Related to https://github.com/hyperledger/besu/pull/7015.

`./gradlew :evm:spotlessJavaApply`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785 

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
        Created At 2024-04-30 23:49:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7024" class=".btn">#7024</a>
            </td>
            <td>
                <b>
                    build - Update license headers formatting (HL 2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

`./gradlew :datatypes:spotlessJavaApply :config:spotlssJavaApply`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785

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
        Created At 2024-04-30 23:27:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7023" class=".btn">#7023</a>
            </td>
            <td>
                <b>
                    Add new acceptance test to soak test BFT chains
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR adds a new long-running acceptance test that is designed as a soak test for BFT chains.

It is disabled by default (i.e. `acceptanceTestCliqueBft` does not run this test) but can be run as an individual acceptance test with `./gradlew acceptanceTestBftSoak`.

The current acceptance test tasks for gradle have not been updated to run the new test to ensure that PRs do not require an hour-long test before being mergeable. It is intended to be run manually by anyone who wants to easily run a soak test of the latest code on a QBFT or IBFT chain. Future discussions with the maintainers might decide to add the test somewhere else in the release pipeline.

By default the test runs for 60 minutes, but can be run for much longer by configuring the `acctests.soakTimeMins` system property in `build.gradle`. It has been tested for runs of up to 6 hours so far.

Here's a summary of what the test does:

1. Creates a 4-validator QBFT chain with `berlin` fork
2. Starts the nodes
3. Deploys a smart contract to create some initial state
4. Attempts to deploy a `shanghai` contract and checks that it fails
5. Lets the chain continue mining empty blocks for a proportion of the total run time (e.g. for a 60 minute run it will do this step for 10 minutes)
   - Every minute it checks that the chain height is increasing, with some tolerance allowed
6. Stops a node and checks the chain continues to mine blocks
   - Again every minute it checks that the chain height is increased, but with more tolerance for the slower mining rate
7. Stops another node and checks the the chain now stalls
8. Starts both of the stopped nodes. Waits for the chain to continue mining blocks again
9. Stops all of the nodes one-by-one, upgrading them from `berlin` to `london` fork
10. Checks that the chain continues mining new blocks once the nodes have restarted
11. Does another check that the state of the smart contract deployed at step 3 is correct (periodic updates are made to the state of the contract in between the other steps so the last check is to make sure the state is correct from the latest update)
12. Upgrades the chain from `london` to `shanghai`
13. Attempts to deploy the `shanghai` contract that failed at step 4 and checks that it was successful

If the test is configured to run for twice as long (e.g. 2 hours) each of the main steps runs for twice as long. The test cannot be configured to run for < 1 hour as the timings for the nodes resyncing & QBFT rounds being agreed upon after the chain has stalled have minimum reliable values. There's not theoretical upper limit to how long the test can run for.

Future additions I'd like to add to the test:
 - ~Upgrade the chain from `london` to `shanghai` and check that the `shanghai` contract is deployed successfully~ Added under the latest commit
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-30 16:37:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7021" class=".btn">#7021</a>
            </td>
            <td>
                <b>
                    build - Update license headers formatting (HL 1)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Related to https://github.com/hyperledger/besu/pull/7015.

`./gradlew :besu:spotlessJavaApply`

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785 

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
        Created At 2024-04-30 11:39:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7020" class=".btn">#7020</a>
            </td>
            <td>
                <b>
                    build - Update license headers formatting (6)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Related to https://github.com/hyperledger/besu/pull/7015.

Fix headers formatting under:
ethereum/ services/

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785 

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
        Created At 2024-04-30 11:08:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7019" class=".btn">#7019</a>
            </td>
            <td>
                <b>
                    build - Update license headers formatting (5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Related to https://github.com/hyperledger/besu/pull/7015.

Fix headers formatting under:
plugin-api/ plugins/

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785 

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
        Created At 2024-04-30 10:53:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7018" class=".btn">#7018</a>
            </td>
            <td>
                <b>
                    build - Update license headers formatting (4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Related to https://github.com/hyperledger/besu/pull/7015.

Fix headers formatting under:
ethereum/

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785 

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
        Created At 2024-04-30 10:47:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7017" class=".btn">#7017</a>
            </td>
            <td>
                <b>
                    build - Update license headers formatting (3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Related to https://github.com/hyperledger/besu/pull/7015.

Fix headers formatting under:
enclave/
evm/
nat/
pki/
util/

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785 

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
        Created At 2024-04-30 10:39:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7016" class=".btn">#7016</a>
            </td>
            <td>
                <b>
                    build - Update license headers formatting (2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Related to https://github.com/hyperledger/besu/pull/7015. 

Fix headers formatting under:
acceptance-tests
config
besu
consensus

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
See #6785 


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
        Created At 2024-04-30 10:32:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7015" class=".btn">#7015</a>
            </td>
            <td>
                <b>
                    build - Preparing spotless license header option and adding license templates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
First part of series of PRs that will streamline license header in Java source files via spotless task. Developers who use IDEs to apply license headers should update their template based on `gradle/spotless/java.current.license` whose copyright notice is copied from https://wiki.hyperledger.org/display/TSC/Copyright+and+License+Policy

Once all the PRs are checked in, developers should be able to perform:
```
./gradlew spotlessCheck
```
and 
```
./gradlew spotlessApply
```

The CI should also report any missing or malformed license headers.
## Related PRs
- https://github.com/hyperledger/besu/pull/7016
- https://github.com/hyperledger/besu/pull/7017
- https://github.com/hyperledger/besu/pull/7018
- https://github.com/hyperledger/besu/pull/7019
- https://github.com/hyperledger/besu/pull/7020
- https://github.com/hyperledger/besu/pull/7021

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
#6785 

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
        Created At 2024-04-30 05:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7012" class=".btn">#7012</a>
            </td>
            <td>
                <b>
                    Refactor genesis config file and options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

While working on optimizing the performance of the startup phase, specifically in regard to genesis file management, I found that there is a bit of tech debt accumulated in the way we manage genesis file and options, that makes it difficult to work with it, and makes the code fragile, so before posting the optimizations, this PR refactors the genesis file management to make it more uniform and also make sure that overrides are always applied, before trying to get any option.

Most of the changed files are related to renaming of change of types, while the core of the refactor is in `BesuCommand`, `BesuController` and `BesuControllerBuilder`.

In `BesuCommand` the genesis file and options are now provided by a supplier, that loads, and caches, them on first request, applying any CLI overrides at load time, and this simplify the workflow, since there is no more ad-hoc code to apply them in different places. Since `GenesisConfigOptions` are always accessible via `GenesisConfigFile` then we can just pass this to the `BesuControllor` simplifying the builder.

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
        Created At 2024-04-29 15:04:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7011" class=".btn">#7011</a>
            </td>
            <td>
                <b>
                    Run apt-get in docker builds without using any cache. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

The  docker build step can fail if `apt-get` gets it's dependencies from a transparent cache (e.g. from an ISP) and this cache serves corrupted or outdated packages. This PR clears all the apt-get cache first and afterwards executes the next steps while making sure that no cache whatsoever is used.

I have further split the the `RUN` command into several steps to make debugging easier, because like that the exact command that is failing while be shown. Right now we have several commands chained together and it's not always clear which of the several commands was failing.

## Fixed Issue(s)
fixes #7009 

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-29 13:29:54 +0000 UTC
    </div>
</div>

