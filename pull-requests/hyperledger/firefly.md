---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    Run E2E tests with matrix including fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It looks like there's a lot of code change here, but it's really not a lot. To summarize the changes:

- Existing E2E tests have been split up into two test suites:
  - `OnChainOffChainTestSuite`
  - `TokensTestSuite`
- There are two "traditional tests" that run these suites
  - `TestEthereumE2ESuite` which runs both suites
  - `TestFabricE2ESuite` which just runs `OnChainOffChainTestSuite`
- The `run.sh` test script has been updated to use several new environment variables which get passed to the CLI to create the appropriate environment.
- The E2E GitHub action now uses a matrix strategy to run each variant of the tests while setting the appropriate environment variables.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 21:15:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/241" class=".btn">#241</a>
            </td>
            <td>
                <b>
                    Add manifest for CLI to pull specific version sets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a manifest file that the CLI will use to pull specific versions of each FireFly microservice. The manifest file can be updated in one of two ways:

- Manually, by hand. If a specific version of a FireFly microservice is needed for the version of FireFly in a specific commit/branch, the manifest can be updated accordingly for that commit/branch 
- Automatically with the script - the `manifestgen.sh` script can be run manually, or with `make manifest` to fetch the latest version of each FireFly microservice.

The script uses the GitHub API to query each repo and get the latest release.

> Note: We should make sure `prerelease` versions are excluded from this.

I will leave this PR in draft state until we actually get images published for all the repos, otherwise the version will be reported as `null`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 21:01:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/240" class=".btn">#240</a>
            </td>
            <td>
                <b>
                    update ui to version 0.3.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 14:27:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/239" class=".btn">#239</a>
            </td>
            <td>
                <b>
                    Add transaction for token transfers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a continuation of #215 with one extra commit to add a transaction for token transfers. Did not want to keep pushing commits onto that one since it's nearly ready to merge.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 18:35:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/237" class=".btn">#237</a>
            </td>
            <td>
                <b>
                    Config key concurrency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a mutex to `configPrefix.keys` to prevent concurrent reading and writing to this map by different goroutines.

- Fixes https://github.com/hyperledger/firefly/issues/235

I also evaluated changing `configPrefix.keys` to be a `sync.Map` https://pkg.go.dev/sync#Map, however I think the change to add a mutex was actually simpler. `sync.Map` has a few disadvantages, one of them being losing type safety. This combined with it actually being a larger code change to use `sync.Map`'s functions to get data in and out of the map, led me to just add the mutex.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 15:31:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Add new unit tests to fix test coverage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 15:07:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/234" class=".btn">#234</a>
            </td>
            <td>
                <b>
                    Capture logs if startup or earlier steps fail
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Per https://github.com/hyperledger/firefly/issues/226#issuecomment-938160813, the change in #231 only helps capture container logs during the test running phase.

If the failure happens during startup or registration in the CLI, then logs aren't currently captured.

This change checks the RC after each step, so that the bash code always goes through the log exit
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 11:56:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/233" class=".btn">#233</a>
            </td>
            <td>
                <b>
                    fix wsclient mocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - artifact left over from wsclient migration to `pkg`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 21:03:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/232" class=".btn">#232</a>
            </td>
            <td>
                <b>
                    Fix new identity checks on registration with confirm=true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes the new registration endpoints so they work with the new identity checks again. With these changes, both the new registration endpoints and the deprecated endpoints (still used by the CLI until https://github.com/hyperledger/firefly-cli/pull/108 goes in) still work too.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 19:36:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/231" class=".btn">#231</a>
            </td>
            <td>
                <b>
                    Capture logs as artifacts even if e2e fails (simulated failure in this commit)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 14:14:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/230" class=".btn">#230</a>
            </td>
            <td>
                <b>
                    Update kin-openapi with fix for #229 and add UT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #229 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 12:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/228" class=".btn">#228</a>
            </td>
            <td>
                <b>
                    make InitialConnectAttempts json tag camel case
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 14:37:26 +0000 UTC
    </div>
</div>

