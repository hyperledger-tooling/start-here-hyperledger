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
                PR <a href="https://github.com/hyperledger/caliper/pull/1427" class=".btn">#1427</a>
            </td>
            <td>
                <b>
                    Distinguish different workers in Prometheus PushGateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The worker index of each worker is added as a label when pushing metrics to PushGateway to distinguish workers.

Fixes #1354 

### Results:

#### /metrics endpoint of PushGateway
![image](https://user-images.githubusercontent.com/36656347/182789819-de441ba3-db97-48e6-8343-c6ac4ff792ba.png)

#### Grafana dashboard showing metrics from two workers simultaneously
![image](https://user-images.githubusercontent.com/36656347/182790028-e23265f3-d2c2-4bdc-9123-e7b2bd8f0f70.png)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 07:34:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1425" class=".btn">#1425</a>
            </td>
            <td>
                <b>
                    Revert "Add workflow for gh-pages branch"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts hyperledger/caliper#1423

This is because the changes were superseded by #1424
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-02 02:37:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1424" class=".btn">#1424</a>
            </td>
            <td>
                <b>
                    Add GitHub Actions workflow for docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* GitHub actions workflows are added to the gh-pages branch
* Issues pointed out by DCI lint are fixed for the latest and vNext docs

This is done because according to [GitHub Docs](https://docs.github.com/en/actions/using-workflows/triggering-a-workflow):
> The following steps occur to trigger a workflow run:
> ...
> 2. GitHub searches the .github/workflows directory in your repository for workflow files that are present **in the associated commit SHA or Git ref of the event**.

So, the workflow file is expected to be present in the gh-pages branch for it to run.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 17:54:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1423" class=".btn">#1423</a>
            </td>
            <td>
                <b>
                    Add workflow for gh-pages branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The dci-lint workflow is added to the workflows executed on PR to the documentation branch.

Closes #1422
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-01 16:51:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1421" class=".btn">#1421</a>
            </td>
            <td>
                <b>
                    Execute integration tests based on changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The integration test workflow is modified to execute only tests that are relevant to the changes made

Closes #1375
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-30 12:38:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1420" class=".btn">#1420</a>
            </td>
            <td>
                <b>
                    Update developer docs for setting up the repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* The developer docs for setting up the repository are updated with the instructions for utilising npm workspaces

Closes #1416
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-30 12:07:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper/pull/1419" class=".btn">#1419</a>
            </td>
            <td>
                <b>
                    Cache docker images across CI workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In this PR:
* Docker images are cached across CI workflows
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-28 16:58:51 +0000 UTC
    </div>
</div>

