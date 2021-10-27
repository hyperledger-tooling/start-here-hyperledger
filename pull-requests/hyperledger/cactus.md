---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1484" class=".btn">#1484</a>
            </td>
            <td>
                <b>
                    feat(iroha): adding checkEmpty param to request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Current functionality did not make use of the newer additional parameter in the Iroha command

Closes: #1265
Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 10:14:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1482" class=".btn">#1482</a>
            </td>
            <td>
                <b>
                    docs(discounted-cartrade): update README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                update README of discounted-cartrade example to reflect changes in ledger setup and script building steps.

resolves: #1428 

Signed-off-by: Izuru Sato <sato.izuru@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 10:45:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1478" class=".btn">#1478</a>
            </td>
            <td>
                <b>
                    style: 2021-09-20 linter warnings batch 9 / 26 #1358
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #1358

Signed-off-by: jgusta <jgustafx@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-23 07:49:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1477" class=".btn">#1477</a>
            </td>
            <td>
                <b>
                    test(test-tooling): filter whitespaces from container logs #1247
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a utility function in the Containers class to stream logs and
automatically exclude newline-only log messages.

Resolves #1247

Signed-off-by: Jake Gustafson <jgustafx@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-23 04:08:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1476" class=".btn">#1476</a>
            </td>
            <td>
                <b>
                    ci: de-couple matrix to separate jobs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ci: de-couple matrix to separate jobs. Resolves #1393

Validations:

* I tested this my making a PR in my own repo and commenting the `tool/ci.sh` and adding small logic to create fail scenario.
* Initial run showing
    * All the build stages/steps
    * With the the temp logic, the build for node v14 fails. 
    <img width="1396" alt="Initial Run with all jobs listed_node_14_failed" src="https://user-images.githubusercontent.com/10603196/138488942-d2038350-7f47-4701-811e-e788f6197f7c.png">

     * The build for node v16 succeeds.
    <img width="1382" alt="Initial Run_node_16_succeded" src="https://user-images.githubusercontent.com/10603196/138489169-6b623be3-6d45-4084-9462-682706215045.png">

* I actually killed the last `build_containers` stage to avoid delay. 
* Once we have the option of re-running all the jobs, if we just click it and re-run all the jobs, it actually pulls down the cache and uses it to decide which steps to run. 
* For Attempt 2, 
    * The build for node v14 still fails because of the additional logic
    <img width="1383" alt="Attempt 2_node_14_still fails" src="https://user-images.githubusercontent.com/10603196/138490268-97e27352-f2b8-4408-a5e0-096eda9f8769.png">

    * For the build for node v16, since the previous run was successful, wherever we had if conditions, it skipped that steps. 
    <img width="1389" alt="Attempt 2_node_16_does not run" src="https://user-images.githubusercontent.com/10603196/138490429-08b2c2f2-8b00-4913-86d4-ec571a2aae2a.png">

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 15:54:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1475" class=".btn">#1475</a>
            </td>
            <td>
                <b>
                    build(yarn): migrate from V1 to V3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We hope to solve issues with this that were plaguing contributors due to
bugs in the much older Yarn 1.x versions that we had to use because Yarn V2
had it's own set of problems when it came to linking the .bin folders for
child packages in a monorepo.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 07:28:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1474" class=".btn">#1474</a>
            </td>
            <td>
                <b>
                    test: skip corda v4.7 deploy test due to flakiness
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Corda</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                Related to #1473 but does NOT fix it, that is to come at a later point
in time when we have time for a full and proper diagnosis+fix.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 04:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1472" class=".btn">#1472</a>
            </td>
            <td>
                <b>
                    test: skip flaky fabric 2.2.x deploy cc from JS test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">Developer_Experience</span><span class="chip">Flaky-Test-Automation</span><span class="chip">Tests</span>
            </td>
            <td>
                This is related to #1471 (does not fix it though). In order to enable
faster CI/PR turnaround times we are aggressively eliminating (skipping)
flaky tests and creating issues in the backlog for fixing them later on.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 22:46:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1470" class=".btn">#1470</a>
            </td>
            <td>
                <b>
                    test(connector-corda): skip deploy-cordapp-jars-to-nodes-v4.8
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Flaky-Test-Automation</span>
            </td>
            <td>
                Related to #1469

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 19:51:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1467" class=".btn">#1467</a>
            </td>
            <td>
                <b>
                    docs: add SECURITY.md file to comply with the HL repo linter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">Security</span>
            </td>
            <td>
                A 100% knockoff of the Fabric project's SECURITY.md file.

Closes: #662
Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 22:44:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1466" class=".btn">#1466</a>
            </td>
            <td>
                <b>
                    build: reset:node-modules script dry-run parameter dropped
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Epic facepalm once again, congratulations to Peter!

The reset:node-modules script had one job, which was to
delete all node_modules directories in the entire repo.
It was on the right track, but the --dry-run flag was forgotten
in among the CLI arguments so this whole time the script was
not working *at all* because of it. Just brilliant... :-)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 22:39:38 +0000 UTC
    </div>
</div>

