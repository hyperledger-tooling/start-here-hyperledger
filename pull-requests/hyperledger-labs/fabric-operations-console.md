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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/279" class=".btn">#279</a>
            </td>
            <td>
                <b>
                    Join Channel Step 2 Next button validation
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

Join Channel Step 2 Next button validation

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 15:04:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    use "bulk_add_components" for a systemless append
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The systemless orderer append flow should use the `bulk_add_components` logic when onboarding and parsing deployer's create-orderer response. This is b/c deployer responds with an array of components and not an object for this route.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-27 13:50:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    Generate Genesis Page Style updates
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

- UI alignment fix


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 15:06:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/276" class=".btn">#276</a>
            </td>
            <td>
                <b>
                    fix route and body for appending to systemless os
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
#### Description
Fixes the route and body to use for the request to append a new orderer node to an os without a system channel.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 14:23:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/275" class=".btn">#275</a>
            </td>
            <td>
                <b>
                    Fix join orderer text alignment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nikhil Modem [nikhil.modem@ibm.com](mailto:nikhil.modem@ibm.com)

#### Type of change

- Bug fix
 
#### Description

- Imported the new joinOSNChanelModal scss to app.scss so that styles are actually applied now.
- Removed the corresponding styles from the channelModal scss file.
- Fixed the alignment of the name of the node and the checkbox to be inline.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 10:40:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    show success toast msg when orderer joins channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
Adds a toast message after a orderer successfully joins the channel using the channel participation apis.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 20:41:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    fix update channel wizard launch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The update channel wizard button was launching the create channel wizard.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-25 20:29:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    Improve msg failed config block
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
If we failed to get a config block b/c of a 503 code, display a better error message.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 20:05:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    Join orderer text
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
- added text to pending channel tile
- fliped osnadmin_feats_enabled feature flag to true


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-22 14:24:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    remove console component auto restarts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
if the `node_ou` field of a component is edited, the console should not send a restart since the operator will already do that


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 19:17:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    prevent blank pending channel tile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
It's possible to create a blank pending channel tile by creating a real tile, and then canceling the create channel wizard right after starting it. This PR prevents any blank pending channel tiles.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 21:05:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    create channel - show error if 0 orderers are in selected msps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Huffman <dshuffma@us.ibm.com>

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Filtering out msps in https://github.com/hyperledger-labs/fabric-operations-console/pull/264  (for the create channel wizard) was the wrong approach.

What we really needed was a warning/error if the user had not selected any MSPs with a known orderer. So with this PR you can select any MSP you want, as long as 1 or more of them have orderers.

This prevents the error we are trying to stop where a user selects MSPs with 0 orderers && leaves the consenter step as `default` and we create a problematic genesis block since it has 0 consenters.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 20:41:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    Bump terser from 4.8.0 to 4.8.1 in /packages/apollo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [terser](https://github.com/terser/terser) from 4.8.0 to 4.8.1.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/terser/terser/blob/master/CHANGELOG.md">terser's changelog</a>.</em></p>
<blockquote>
<h2>v4.8.1 (backport)</h2>
<ul>
<li>Security fix for RegExps that should not be evaluated (regexp DDOS)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/terser/terser/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=terser&package-manager=npm_and_yarn&previous-version=4.8.0&new-version=4.8.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-20 18:32:12 +0000 UTC
    </div>
</div>

