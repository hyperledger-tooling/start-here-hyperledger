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
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1518" class=".btn">#1518</a>
            </td>
            <td>
                <b>
                    Bump normalize-url from 4.5.0 to 4.5.1 in /examples/supplychain-app/quorum/express_nodeJS
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
        Created At 2021-06-11 00:21:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1517" class=".btn">#1517</a>
            </td>
            <td>
                <b>
                    [shared] only TLS 1.2+ allowed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: pppazos <hgartti@gmail.com>

**Changelog**
- Add default TLSContext for ambassador
- Add min_tls_version: v1.2 in all Ambassador TLSContext objects
- Remove ELBSecurityPolicy-TLS-1-2-2017-01 annotation

 

**Reviewed by**
@sownak @suvajit-sarkar 

 

**Linked issue**
#1500 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 06:27:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1516" class=".btn">#1516</a>
            </td>
            <td>
                <b>
                    [quorum] implemented new test for create/crypto/raft rol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: mgCepeda <marina.gomez.cepeda@accenture.com>

**Changelog**
- Add new test for create/crypto/raft rol
- Fixed task using molecule-idempotence-notest tag to be able to run the implemented test

 

**Reviewed by**
@suvajit-sarkar
@alvaropicazo

 

**Linked issue**
#720 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 10:55:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1515" class=".btn">#1515</a>
            </td>
            <td>
                <b>
                    [shared] update AWS cli to v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Update aws cli to v2

 

**Reviewed by**
@sownak 
 

**Linked issue**
#1514

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-08 10:27:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1505" class=".btn">#1505</a>
            </td>
            <td>
                <b>
                    [besu] Adding new validator node to existing network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

Signed-off-by: alvaropicazo <alvaro.picazo.haase@accenture.com>

**Changelog**
- Added validator_node role for creating new enode, certs and doing the voting process by existing validator nodes
- Fixed create/ambassador nested_main condition
- Updated docs for new role

 

**Reviewed by**
@jagpreetsinghsasan 
@suvajit-sarkar

 

**Linked issue**
#1494 

**Screenshots**

![Capture1](https://user-images.githubusercontent.com/76157062/121003315-b1aaa980-c78d-11eb-923c-586ff8aff580.PNG)

Helm releases files are updated correctly with all the static nodes
![Capture2](https://user-images.githubusercontent.com/76157062/121003380-c1c28900-c78d-11eb-8e28-9a7bca041af0.PNG)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 10:44:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1504" class=".btn">#1504</a>
            </td>
            <td>
                <b>
                    [corda-ent] remove ambassador license
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Changelog**
- remove ambassador license
- Update jenkinsfile for corda-ent


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 10:39:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1503" class=".btn">#1503</a>
            </td>
            <td>
                <b>
                    [shared] Changed default namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: angelaalagbe <angela.alagbe@accenture.com>

**Changelog**
- Updated default namespace to component_ns

 

**Reviewed by**
@suvajit-sarkar @sownak 

 

**Linked issue**
#1491 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 11:32:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-automation-framework/pull/1502" class=".btn">#1502</a>
            </td>
            <td>
                <b>
                    [docs] Using GitHub API icons for roadmap
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: suvajit-sarkar <suvajit.sarkar@accenture.com>

**Changelog**
- Removed roadmap icons from _static folder
- Update roadmap icons to use github icons url 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-04 08:14:18 +0000 UTC
    </div>
</div>

