---
layout: default
title: fabric-test
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-test
---

# fabric-test <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-test){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/405" class=".btn">#405</a>
            </td>
            <td>
                <b>
                    Remove caliper daily test as it's broken anyway (backport #404)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">conflicts</span>
            </td>
            <td>
                This is an automatic backport of pull request #404 done by [Mergify](https://mergify.com).
Cherry-pick of b64477cdc99edb20be80b50be3e0ae1f9ecbff07 has failed:
```
On branch mergify/bp/release-2.4/pr-404
Your branch is up to date with 'origin/release-2.4'.

You are currently cherry-picking commit b64477cd.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes to be committed:
	modified:   ci/azure-pipelines-daily.yml
	deleted:    ci/templates/install_deps_caliper.yml
	deleted:    regression/barebones_caliper/barebones_suite_test.go
	deleted:    regression/barebones_caliper/barebones_test.go
	deleted:    regression/barebones_caliper/benchmarks/callbacks/barebonesCreateAsset.js
	deleted:    regression/barebones_caliper/benchmarks/config_barebones.yaml

Unmerged paths:
  (use "git add/rm <file>..." as appropriate to mark resolution)
	both modified:   Makefile
	deleted by them: regression/barebones_caliper/go.mod
	deleted by them: regression/barebones_caliper/go.sum

```


To fix up this pull request, you can check it out locally. See documentation: https://docs.github.com/en/github/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/checking-out-pull-requests-locally

---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 18:37:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/404" class=".btn">#404</a>
            </td>
            <td>
                <b>
                    Remove caliper daily test as it's broken anyway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 17:03:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    Remove Kafka from orderer.yaml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Kafka was removed from the main branch of the fabric core

Signed-off-by: yacovm <yacovm@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 12:17:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    add the verbose flag to node test runs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Matthew B White <whitemat@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 15:18:00 +0000 UTC
    </div>
</div>

