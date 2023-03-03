---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    set read only first
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
During migration we should put the console in the read only state first and not last. This will prevent the creation of opensource style components on saas.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 17:53:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    fixes the migrated endpoints for k8s clusters only
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

Fixes building the endpoints for k8s clusters.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 13:32:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    bump release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->


- Documentation update

#### Description
increment release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 22:30:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    use deployer api to set infrastructure setting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
use the new deployer api to set infrastructure setting.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 22:23:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    add minimum stream logic for migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)


#### Description
add minimum stream logic for migration


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 21:19:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    Add endpoint to determine if clustertype is openshift or k8s
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix
- Improvement

#### Description
* A new endpoint `/api/v3/instance/{serviceInstanceID}/cluster/type` to determine if the cluster is ocp or k8s 
* Added a fix to override endpoints for k8s only and unchange ocp endpoints


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 20:59:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    build the legacy field backend_addr last
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Fixes setting the legacy field  `backend_addr` in component docs.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 20:23:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/396" class=".btn">#396</a>
            </td>
            <td>
                <b>
                    disable more buttons if in read only mode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
A few buttons were left enabled, this disables them when the console is in read-only mode.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 17:44:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/395" class=".btn">#395</a>
            </td>
            <td>
                <b>
                    fix urls of migrated components by adding migrated flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Migrated components need the migrated flag added, else it doesn't use the right url.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 17:27:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/394" class=".btn">#394</a>
            </td>
            <td>
                <b>
                    fix permission error related to /iam/info api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Fixes the IAM permission error on the `/iam/info` api.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 16:34:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/393" class=".btn">#393</a>
            </td>
            <td>
                <b>
                    disable buttons if read only is true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
If read only mode is enabled, the actions buttons will be disabled or hidden. The apis are already disabled and will error if used, this just make's it prettier but not letting a user click a button.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 22:14:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/392" class=".btn">#392</a>
            </td>
            <td>
                <b>
                    remove code blocking "bad" fabric images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
This PR allows selecting the "bad" fabric images. Which were all v2.2.9s, and v2.2.8-3.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 14:41:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/391" class=".btn">#391</a>
            </td>
            <td>
                <b>
                    edit component docs prior to migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The MSP docs and the signature collection docs need to be edited prior to migration.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-28 14:12:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/390" class=".btn">#390</a>
            </td>
            <td>
                <b>
                    open source support contact removal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix


#### Description
<!--- Describe your changes in detail, including motivation. -->

open source support contact removal

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 08:23:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/388" class=".btn">#388</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/sys from 0.0.0-20220209214540-3681064d5158 to 0.1.0 in /packages/fabric-deployer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [golang.org/x/sys](https://github.com/golang/sys) from 0.0.0-20220209214540-3681064d5158 to 0.1.0.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/golang/sys/commits/v0.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/sys&package-manager=go_modules&previous-version=0.0.0-20220209214540-3681064d5158&new-version=0.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-25 11:27:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/387" class=".btn">#387</a>
            </td>
            <td>
                <b>
                    show warning msg if selected version breaks node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->
- Improvement (improvement to code, performance, etc)

#### Description
This PR adds a warning message if the peer version selected during upgrade, or when creating a new peer, can break older node.js chaincode.

This effects peer versions: 2.2.9s, 2.2.8-3, and any 2.4s.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-24 21:18:39 +0000 UTC
    </div>
</div>

