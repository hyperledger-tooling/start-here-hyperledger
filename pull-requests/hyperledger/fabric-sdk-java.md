---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    Simplify pull request checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a job to the end of the pull_request workflow that depends on the build jobs, and can be used as a single job to check pull request success. This avoids the need to change the branch protection PR checks when changes are made to the build process.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-19 11:04:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    Update build status images in README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Scheduled builds are now run in GitHub Actions, not Azure Pipelines.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-16 12:11:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    Update opentelemetry to 1.22.0 (backport #250)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #250 done by [Mergify](https://mergify.com).


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
        Created At 2023-01-16 11:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/251" class=".btn">#251</a>
            </td>
            <td>
                <b>
                    Use GitHub Actions for build (release-1.4)
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
        Created At 2023-01-13 21:50:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/250" class=".btn">#250</a>
            </td>
            <td>
                <b>
                    Update opentelemetry to 1.22.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update to the latest existing opentelemetry version 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-13 16:36:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    Use callable workflow from release-2.2 branch in scheduled builds
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
        Created At 2023-01-12 16:36:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    Refactor CI pipeline (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Split tests to callable workflow to enable multi-release scheduled builds
- Automatic cancel of in-progress pull request builds on a new push
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-12 13:36:20 +0000 UTC
    </div>
</div>

