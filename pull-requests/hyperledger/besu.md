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
                PR <a href="https://github.com/hyperledger/besu/pull/7245" class=".btn">#7245</a>
            </td>
            <td>
                <b>
                    Make code sizes a characteristic of the EVM version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Make the max code size and max initcode size a part of the EVM configuration. As part of the change we need to move the tasks CodeFactory once handled as a static class and move it into the EVM. This has a nice follow on effect that we don't need to pass in max EOF versions or max code sizes anymore.

This is also required to address a recent EOF change limiting the total size of containers.

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
        Created At 2024-06-19 17:25:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7239" class=".btn">#7239</a>
            </td>
            <td>
                <b>
                    container verify GitHub workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Container verification step in release process automated with the container verify GitHub workflow. New workflow is triggered at the end of the release workflow which will check the released container images starts successfully. Verification test only checks container starts and reach the Ethereum main loop.

## Fixed Issue(s)
fixes #7176

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
        Created At 2024-06-18 23:05:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7237" class=".btn">#7237</a>
            </td>
            <td>
                <b>
                    EIP 7702
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

## Fixed Issue(s)
fixes #7205 


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
        Created At 2024-06-18 14:07:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7234" class=".btn">#7234</a>
            </td>
            <td>
                <b>
                    fix: workflow permission to upload trivy sarif report
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Trivy scan result upload to GitHub fails due to permission issue. Added permission security-events=write to the workflow file as a fix. Since workflow permission explicitly defined, it requires contents=read explicity set as well

## Fixed Issue(s)

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [x] acceptance tests: `./gradlew acceptanceTest`
- [x] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 01:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7233" class=".btn">#7233</a>
            </td>
            <td>
                <b>
                    check initcode size earlier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

Fail earlier with the initcode size check

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
        Created At 2024-06-16 00:33:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7232" class=".btn">#7232</a>
            </td>
            <td>
                <b>
                    Check for EOFCreate subcontainer rules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Check and test for the unused container rule, and only returncontract
targets can have truncated data rule.
Also test the other subcontainer rules in unit tests.

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
        Created At 2024-06-14 04:19:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7231" class=".btn">#7231</a>
            </td>
            <td>
                <b>
                    fix: update artifacts hash on release page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Release workflow publish step was missing the depepndency of artifacts jobs. Due to this reason it could not collect the artifact hashes from the artifacts job. This was introduced in the release workflow consolidation

## Fixed Issue(s)
fixes #7229


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
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
        Created At 2024-06-14 04:02:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7230" class=".btn">#7230</a>
            </td>
            <td>
                <b>
                    Changelog download links for 24.6.0 release and next release changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add download links to 24.6.0 release and move changelog entries after 24.6.0 to next release section.

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
        Created At 2024-06-14 03:52:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7228" class=".btn">#7228</a>
            </td>
            <td>
                <b>
                    fix: pin github actions in container security scan workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Repository follow standard to use git hash to pin the GitHub actions. Updated the container security scan workflow actions with their git hashes.

## Fixed Issue(s)
fix requested in [discord](https://discord.com/channels/905194001349627914/905205502940696607/1250837893040177175) message

### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
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
        Created At 2024-06-13 21:18:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7227" class=".btn">#7227</a>
            </td>
            <td>
                <b>
                    Temporary CancunEOF fork for EOF testing.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add Genesis ("CancunEOFTime") and reference test ("CancunEOF") support
for a temporary Cancun+EOF fork, in anticipation of potential devnets.

Signed-off-by: Danno Ferrin <danno@numisight.com>

## PR description

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
        Created At 2024-06-13 19:12:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7226" class=".btn">#7226</a>
            </td>
            <td>
                <b>
                    chore: fix typos in changelog
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- This PR fixes some typos found in the changelog


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 14:36:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7223" class=".btn">#7223</a>
            </td>
            <td>
                <b>
                    feat: Add network option for LUKSO Mainnet
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

This PR provides an option to connect to [LUKSO Mainnet](https://www.lukso.network/) network, using `--network=lukso` flag.

## Fixed Issue(s)

No matching issues 

### Thanks for sending a pull request! Have you done the following?

- [X] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [X] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [X] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 09:24:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7222" class=".btn">#7222</a>
            </td>
            <td>
                <b>
                    Add build version option to prefix git hash with custom version property
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Adds the option to provide a custom version prefix at build time that will be prefixed to the git hash. Currently a custom version can't include the githash. This follows on from some recent version refactoring in https://github.com/hyperledger/besu/pull/6699

Specifically it allows for `-Pversionprefix=24.5.2` to result in a version like `v24.5.2-16ff080`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-13 09:04:22 +0000 UTC
    </div>
</div>

