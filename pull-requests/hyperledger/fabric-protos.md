---
layout: default
title: fabric-protos
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-protos
---

# fabric-protos <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-protos){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/108" class=".btn">#108</a>
            </td>
            <td>
                <b>
                    Allow release builds to be re-run manually
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It would be useful to rerun the release build using the workflow_dispatch event, however this does not currently work because the workflows are checking the github ref for a v* version tag.

It’s not safe to always publish for a manual build and all the language bindings at a particular version should be published from the same commit, so this PR adds a job to the ci-checks workflow to look for the required version tag on the commit being built.

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 15:17:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Allow Maven after Github fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 13:20:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    Use base64 encoded deploy key
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The key works locally but fails in the build for some reason…

```
Load key "/home/runner/.ssh/fabric-protos-go-apiv2_deploy_key": invalid format
```

Try using a base64 encoded key instead

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 10:14:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/105" class=".btn">#105</a>
            </td>
            <td>
                <b>
                    Explicitly install and use Go 1.18 in GitHub Actions
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
        Created At 2022-06-15 10:01:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/104" class=".btn">#104</a>
            </td>
            <td>
                <b>
                    Bump version to 0.1.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:20:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/103" class=".btn">#103</a>
            </td>
            <td>
                <b>
                    Fix path to installDeployKey.sh script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Build failed to find the script due to working-directory being publish-apiv2

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 08:20:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/101" class=".btn">#101</a>
            </td>
            <td>
                <b>
                    Use deploy key to publish Go apiv2 bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previous publish failed with permission denied

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 16:28:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/100" class=".btn">#100</a>
            </td>
            <td>
                <b>
                    Publish Go apiv2 bindings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Push a generated Go bindings commit to hyperledger/fabric-protos-go-apiv2 repo for every push to the fabric-protos main branch

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-14 11:32:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-protos/pull/99" class=".btn">#99</a>
            </td>
            <td>
                <b>
                    Use bot email
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Switch from placeholder email.

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 21:37:57 +0000 UTC
    </div>
</div>

