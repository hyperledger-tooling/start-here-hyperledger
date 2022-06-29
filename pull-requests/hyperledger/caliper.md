---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1394" class=".btn">#1394</a>
            </td>
            <td>
                <b>
                    [WIP] Migrate to npm workspaces
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The repository is migrated from lerna to npm workspaces

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 14:03:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1393" class=".btn">#1393</a>
            </td>
            <td>
                <b>
                    Add DCI linting to CI of PRs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As recommended by the project update template and https://github.com/petermetz/gh-action-dci-lint
Let's see whether the remnant phrases in the changelog and third-party artifacts will trigger the alarm before making this a branch protection rule.

Signed-off-by: Attila Klenik <a.klenik@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-28 11:25:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1391" class=".btn">#1391</a>
            </td>
            <td>
                <b>
                    Fix#1377 Change the generator binding from 2.2 to 1.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tezas-6174 <jamdade.2@iitj.ac.in>

- Fixes #1377.
- Changed the generator binding from 2.2 to 1.4 in ``run.sh`` in generator-tests of ``caliper-test-integration`` package.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-26 15:19:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1390" class=".btn">#1390</a>
            </td>
            <td>
                <b>
                    Pass secrets to CI workflow for publish
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* Secrets are passed on from the parent workflow to the publish workflow as described in the GitHub Actions documentation

Fixes #1389

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-26 11:16:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1387" class=".btn">#1387</a>
            </td>
            <td>
                <b>
                    Cache node modules across CI workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The `node_modules` folder is cached across workflows using a method inspired by the workflow in [jupyterlab/extension-examples](https://github.com/jupyterlab/extension-examples/blob/master/.github/workflows/main.yml)

Closes #1374

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 17:42:44 +0000 UTC
    </div>
</div>

