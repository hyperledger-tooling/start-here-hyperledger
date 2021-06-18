---
layout: default
title: blockchain-automation-framework
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-automation-framework
---

# blockchain-automation-framework <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-automation-framework){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1533" class=".btn">#1533</a>
            </td>
            <td>
                <b>
                    [quorum] fixed molecule test errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Fixed quorum crypto-ibft molecule test errors
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 19:54:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1532" class=".btn">#1532</a>
            </td>
            <td>
                <b>
                    [indy] fix docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Update versions for software in docs
- Fix empty cacert file
- Update default ambassador ports

 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 16:27:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1531" class=".btn">#1531</a>
            </td>
            <td>
                <b>
                    [besu] create orion crypto using helmcharts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

**Changelog**
- Add orion_crypto helmchart
- Fix orion binary problem
- Update ansible to use orion-job to create orion crypto
- Remove -bes from folder structure


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 10:02:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1530" class=".btn">#1530</a>
            </td>
            <td>
                <b>
                    [besu] Adding a new validator organization with multiple nodes to existing network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- Added validator-new-org network.yaml sample
- Fixed what was causing the restart of the existing validator nodes (their value files were being updated and that is not supposed to happen).
- Updated validator_node role for supporting the addition of a new validator node in an existing org to an existing network and the addition of a new validator org with one or multiple validator nodes.

 

**Reviewed by**
@suvajit-sarkar 
@jagpreetsinghsasan 
@sownak 

 

**Linked issue**
#1017

*Screenshots*

![all-validators](https://user-images.githubusercontent.com/76157062/122366131-91cc7000-cf5b-11eb-91a3-12c8c863e70f.PNG)

After the add-validator playbook finished, a new validator org was added (ssalv-bes) containing two validator nodes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 09:03:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1529" class=".btn">#1529</a>
            </td>
            <td>
                <b>
                    [quorum] changed namespace in my converge and prepare, edited verify in parall…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …el with these changes

Signed-off-by: Angela Alagbe <angela.alagbe@accenture.com>

**Changelog**
- Add idempotence notest to nested main
- Fixed bug
- Updated verify.yaml

 

**Reviewed by**
@suvajit-sarkar 

 

**Linked issue**
#1527 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 08:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1528" class=".btn">#1528</a>
            </td>
            <td>
                <b>
                    [shared] cleanup share versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- add default versions on shared roles and cleanup playbooks for:
    - **setup/kubectl** :  default in defaults/main.yaml to 1.16.3, can be override from playbook
    - **setup/helm**   default in defaults/main.yaml to v3.2.4, can be override from playbook
    - **setup/vault** default in defaults/main.yaml to v1.7.0, can be override from playbook
    - **setup/aws-auth** default in defaults/main.yaml to v1.10.3, can be override from playbook
    - **setup/ambassador** version is locked in helm chart


**Reviewed by**
@sownak , @suvajit-sarkar 

 

**Linked issue**
#1511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-17 06:48:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1526" class=".btn">#1526</a>
            </td>
            <td>
                <b>
                    [quorum] Added constellation prereq. in the molecule test workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Add required libraries in molecule test workflow
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 10:15:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1525" class=".btn">#1525</a>
            </td>
            <td>
                <b>
                    [quorum] Implemented test for create/tessera rol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add new test for create/tessera rol
- Fixed task using molecule-idempotence-notest tag or changed_when: false to be able to run the implemented test
 

**Reviewed by**
@suvajit-sarkar
@alvaropicazo

 
**Linked issue**
#724 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-14 13:47:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1522" class=".btn">#1522</a>
            </td>
            <td>
                <b>
                    [shared] merge from master
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
fix security issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 13:35:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1521" class=".btn">#1521</a>
            </td>
            <td>
                <b>
                    [fabric] upgrade versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roy,Sownak <sownak.roy@accenture.com>

Fix security alerts
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 13:10:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1520" class=".btn">#1520</a>
            </td>
            <td>
                <b>
                    Bump normalize-url from 4.5.0 to 4.5.1 in /examples/supplychain-app/besu/smartContracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [normalize-url](https://github.com/sindresorhus/normalize-url) from 4.5.0 to 4.5.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/sindresorhus/normalize-url/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=normalize-url&package-manager=npm_and_yarn&previous-version=4.5.0&new-version=4.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-automation-framework/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 10:19:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1519" class=".btn">#1519</a>
            </td>
            <td>
                <b>
                    Bump normalize-url from 4.5.0 to 4.5.1 in /examples/supplychain-app/quorum/smartContracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [normalize-url](https://github.com/sindresorhus/normalize-url) from 4.5.0 to 4.5.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/sindresorhus/normalize-url/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=normalize-url&package-manager=npm_and_yarn&previous-version=4.5.0&new-version=4.5.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-automation-framework/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 07:43:08 +0000 UTC
    </div>
</div>

