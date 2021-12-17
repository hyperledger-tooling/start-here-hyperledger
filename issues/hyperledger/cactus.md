---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1469" class=".btn">1469</a>
            </td>
            <td>
                <b>
                    test(connector-corda): fix flaky v4.8 test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">Corda</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                **Describe the bug**

We've got a flaky one at:
packages/cactus-plugin-ledger-connector-corda/src/test/typescript/integration/deploy-cordapp-jars-to-nodes-v4.8.test.ts

One of the corda nodes within the container occasionally don't boot up (hangs and then the test waits for an hour before giving up).

**To Reproduce**

Keep running the test and eventually you'll see it.

**Expected behavior**

Tests are stable, not flaky.

**Logs/Stack traces**

The CI logs from the GHA runner as of this morning:
[logs_10155.zip](https://github.com/hyperledger/cactus/files/7392356/logs_10155.zip)

**Cloud provider or hardware configuration:**

GHA runner

**Operating system name, version, build:**

Ubuntu 20.04

**Hyperledger Cactus release version or commit (git rev-parse --short HEAD):**

1.0.0-rc.1

**Hyperledger Cactus Plugins/Connectors Used**

Corda

**Additional context**

I'll send a separate PR that skips this test to avoid flakiness in the meantime.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 19:33:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1461" class=".btn">1461</a>
            </td>
            <td>
                <b>
                    fix(key-converter): Files needs to migrated from Tape to Jest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">Nice-to-Have</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span>
            </td>
            <td>
                **Describe the bug**

Test file, key-converter, has multiple methods that are being skipped. 

**Expected behavior**

The test file should be able to run without it's methods having to be skipped.

**File Path:** packages/cactus-common/src/test/typescript/unit/key-converter.test.ts

**After Correction**
Migrate file from Tape to Jest.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 15:33:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1386" class=".btn">1386</a>
            </td>
            <td>
                <b>
                    test(connector-besu): fix missing multi-party all-in-one ledger image caching
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">Nice-to-Have</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Performance</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span>
            </td>
            <td>
                > This is marked as a good first issue because mostly you just need to be experienced in containerization, not necessarily the core of the Cactus code nor distributed ledgers. Do bear in mind that it is level 400 though so it's not exactly easy unless you have significant experience with containers.

**Describe the bug**

The  multi-party all-in-one ledger image for Besu tests does not cache the images it downloads from DockerHub, meaning that every time the tests run it pulls all the images again and this has been leading to rate limiting errors that make the CI flaky (once again)

**To Reproduce**

Run a lot of tests for a lot of PRs all at once and in a few hours you will have exhausted the DockerHub rate limit and all the tests will start failing for the next 6-12 hours until the rate limit cools off.

**Expected behavior**

Tests are stable, DockerHub rate limits are not at risk of being hit at any time regardless of how many tests we run in parallel. 

Either the AIO besu multi-party image caches a set of pinned versions of all the images it uses (e.g. fetches from dockerhub) at image **build** time so that by the time the CI pulls up the container for the tests, it only needs to download the one big image from ghcr.io instead of dockerhub (the former does not have rate limits - yet)

Relevant Dockerfile:
`tools/docker/besu-multi-party-all-in-one/Dockerfile`

**Logs/Stack traces**

N/A

**Screenshots**

N/A

**Cloud provider or hardware configuration:**

GH managed action runners

**Operating system name, version, build:**

Ubuntu 20.04

**Hyperledger Cactus release version or commit (git rev-parse --short HEAD):**

0.9.0 / 0.10.0

**Hyperledger Cactus Plugins/Connectors Used**

Besu

**Additional context**

The AIO besu multi-party image caches a set of pinned versions of all the images it uses

Relevant Dockerfile:
`tools/docker/besu-multi-party-all-in-one/Dockerfile`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-28 00:52:43 +0000 UTC
    </div>
</div>

