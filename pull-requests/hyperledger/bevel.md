---
layout: default
title: bevel
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/bevel
---

# bevel <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/bevel){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2279" class=".btn">#2279</a>
            </td>
            <td>
                <b>
                    [chore] add missing commits
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
        Created At 2023-06-01 15:58:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2278" class=".btn">#2278</a>
            </td>
            <td>
                <b>
                    [chore] release v0.14.0 merge
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
        Created At 2023-06-01 15:46:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2277" class=".btn">#2277</a>
            </td>
            <td>
                <b>
                    [chore] merged from main
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
        Created At 2023-06-01 15:34:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2276" class=".btn">#2276</a>
            </td>
            <td>
                <b>
                    [chore] merge from develop
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
        Created At 2023-06-01 15:11:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2275" class=".btn">#2275</a>
            </td>
            <td>
                <b>
                    [chore] add release tags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Change log**

- update roadmap
- update charts version with release tags
- update appVersion for besu charts
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 14:19:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2274" class=".btn">#2274</a>
            </td>
            <td>
                <b>
                    [ci-skip] Fixed add org for proxy none
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added fix for add-org not working when proxy == none
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 17:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2272" class=".btn">#2272</a>
            </td>
            <td>
                <b>
                    [besu] improve error handling mechanism for vault api calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

feat(besu): improve error handling mechanism for vault api calls

```
This pull request introduces improvements to the error handling mechanism and enhances troubleshooting capabilities in the bevel-vault.sh script. The changes made include:

 • Implemented error handling at the individual function level.
 • Enhanced error message logging for better visibility into failures.
 • Improved error checking and validation.
 • Updated paths in respect of the function calls to reflect the latest changes.
```

fixes #2260
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 12:37:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2271" class=".btn">#2271</a>
            </td>
            <td>
                <b>
                    [shared] Add chart release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added `release_charts.yml` Github Action to release charts. This automatically updates the gh-pages as well. To trigger this workflow correctly, the Chart versions need to be updated, as demonstrated in the update for Fabric charts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 15:07:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2270" class=".btn">#2270</a>
            </td>
            <td>
                <b>
                    [besu] update path for generating cactus-connector helm release file.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---
bug(besu): update path for generating cactus-connector helm release file
```
Description:

- The generated Helm release file for the Cactus connector is currently not stored in its own organization directory within the release folder for the Besu platform. As a result, improper resetting of the entire Besu network occurs.
- This pull request proposes an update to the path, ensuring that the cactus-connector Helm release file is generated within the respective organizations.

Solution:

- Update the path for generating the cactus-connector Helm release file to the appropriate organization directory within the release folder for the Besu platform.
- This adjustment will enable successful deletion and resetting of the Besu network.

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 12:26:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2269" class=".btn">#2269</a>
            </td>
            <td>
                <b>
                    [ci-skip] deploy Besu Cactus connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

**docs(besu): deploy Besu Cactus connector**

```
• This commit adds a guide for deploying the Besu Cactus connector. It includes instructions for modifying the configuration 
  file to enable the connector for validators and peers, as well as running the playbook to deploy the connector.
• The guide provides step-by-step instructions and highlights the prerequisites for deploying the Cactus connector. It also 
  includes a reference to a sample configuration file for easy customization.
• This commit aims to improve the documentation and enable users to deploy the Cactus connector effectively in their Besu 
  networks.

```
fixes #2250
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 13:25:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2268" class=".btn">#2268</a>
            </td>
            <td>
                <b>
                    [ci-skip] hot fixes: added k8s config file path in setup/vault-script …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Added k8s config file path in setup/vault-script role

Modifications
-------------
platforms/hyperledger-besu/configuration/deploy-network.yaml
platforms/shared/configuration/roles/setup/vault-script/tasks/main.yml

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 12:57:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2267" class=".btn">#2267</a>
            </td>
            <td>
                <b>
                    [ci-skip] Create operation guide on deploying cacti connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
--------------
1. Added operation guide on deploying fabric cacti connector

Modifications in docs
-----------------------
docs/source/operationalguide.rst
docs/source/operations/setup_cactus_connector_fabric.md
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 08:44:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2264" class=".btn">#2264</a>
            </td>
            <td>
                <b>
                    Fix formatting in contributing guidelines
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes issue #2242
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 04:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2263" class=".btn">#2263</a>
            </td>
            <td>
                <b>
                    [besu] improve error handling mechanism for vault api calls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit to be reviewed**
---

feat(besu): improve error handling mechanism for vault api calls

```
This pull request introduces improvements to the error handling mechanism and enhances troubleshooting capabilities in the bevel-vault.sh script. The changes made include:
 • Implemented error handling at the individual function level.
 • Enhanced error message logging for better visibility into failures.
 • Improved error checking and validation.
 • Updated paths in respect of the function calls to reflect the latest changes.
```

fixes #2260
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 11:51:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/bevel/pull/2262" class=".btn">#2262</a>
            </td>
            <td>
                <b>
                    [substrate] Update chart readme's
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Added readme and updated Chart.yaml so that the helm charts can be made available as a repo.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 11:47:31 +0000 UTC
    </div>
</div>

