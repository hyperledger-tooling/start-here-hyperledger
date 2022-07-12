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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    fix empty channel list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Varad Ramamoorthy <varad@us.ibm.com>

#### Type of change
- Bug fix


#### Description
Channel list is empty when there are channels with empty OrdererAddresses


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 15:58:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    updated release notes
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
- Documentation update

#### Description
release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 20:37:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    improve system channel readme
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

- Documentation update

#### Description
Added a `Console differences with no system channel` section


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 20:28:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    add error msg when there are 0 channels for join
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
Added error message when doing a osn admin join and there are no channels to use.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 19:36:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    remove auto restart when editing specific fields
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
The operator will take care of restarting the component when the admin_certs field is edited. This PR removes the restart from console.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 18:59:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    Various system channel fixes
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
- toggle create wizard steps based on systemless status if the drop down selection changes
- add consenter warning to create wizard summary when 0 consenters are found/selected
- fix importing of  asystemless ordering clusters from json
- hide the unjoin channel button on ordering clusters w/system channel (it won't work)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 18:53:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    Bump moment from 2.29.2 to 2.29.4 in /packages/apollo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [moment](https://github.com/moment/moment) from 2.29.2 to 2.29.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/moment/moment/blob/develop/CHANGELOG.md">moment's changelog</a>.</em></p>
<blockquote>
<h3>2.29.4</h3>
<ul>
<li>Release Jul 6, 2022
<ul>
<li><a href="https://github-redirect.dependabot.com/moment/moment/pull/6015">#6015</a> [bugfix] Fix ReDoS in preprocessRFC2822 regex</li>
</ul>
</li>
</ul>
<h3>2.29.3 <a href="https://gist.github.com/ichernev/edebd440f49adcaec72e5e77b791d8be">Full changelog</a></h3>
<ul>
<li>Release Apr 17, 2022
<ul>
<li><a href="https://github-redirect.dependabot.com/moment/moment/pull/5995">#5995</a> [bugfix] Remove const usage</li>
<li><a href="https://github-redirect.dependabot.com/moment/moment/pull/5990">#5990</a> misc: fix advisory link</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moment/moment/commit/000ac1800e620f770f4eb31b5ae908f6167b0ab2"><code>000ac18</code></a> Build 2.24.4</li>
<li><a href="https://github.com/moment/moment/commit/f2006b647939466f4f403721b8c7816d844c038c"><code>f2006b6</code></a> Bump version to 2.24.4</li>
<li><a href="https://github.com/moment/moment/commit/536ad0c348f2f99009755698f491080757a48221"><code>536ad0c</code></a> Update changelog for 2.29.4</li>
<li><a href="https://github.com/moment/moment/commit/9a3b5894f3d5d602948ac8a02e4ee528a49ca3a3"><code>9a3b589</code></a> [bugfix] Fix redos in preprocessRFC2822 regex (<a href="https://github-redirect.dependabot.com/moment/moment/issues/6015">#6015</a>)</li>
<li><a href="https://github.com/moment/moment/commit/6374fd860aeff75e6c9d9d11540c6b22bc7ef175"><code>6374fd8</code></a> Merge branch 'master' into develop</li>
<li><a href="https://github.com/moment/moment/commit/b4e615307ee350b58ac9899e3587ce43972b0753"><code>b4e6153</code></a> Revert &quot;[bugfix] Fix redos in preprocessRFC2822 regex (<a href="https://github-redirect.dependabot.com/moment/moment/issues/6015">#6015</a>)&quot;</li>
<li><a href="https://github.com/moment/moment/commit/7aebb1617fc9bced87ab6bc4c317644019b23ce7"><code>7aebb16</code></a> [bugfix] Fix redos in preprocessRFC2822 regex (<a href="https://github-redirect.dependabot.com/moment/moment/issues/6015">#6015</a>)</li>
<li><a href="https://github.com/moment/moment/commit/57c90622e402c929504cc6d6f3de4ebe2a9ffc73"><code>57c9062</code></a> Build 2.29.3</li>
<li><a href="https://github.com/moment/moment/commit/aaf50b6bca4075f40a3372c291ae8072fb4e9dcf"><code>aaf50b6</code></a> Fixup release complaints</li>
<li><a href="https://github.com/moment/moment/commit/26f4aef9ca0b4c998107bf7e2cf1c33c30368d44"><code>26f4aef</code></a> Bump version to 2.29.3</li>
<li>Additional commits viewable in <a href="https://github.com/moment/moment/compare/2.29.2...2.29.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=moment&package-manager=npm_and_yarn&previous-version=2.29.2&new-version=2.29.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2022-07-07 21:04:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    npm dep updates
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

- Dependency updates

#### Description
<!--- Describe your changes in detail, including motivation. -->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 20:56:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/251" class=".btn">#251</a>
            </td>
            <td>
                <b>
                    add logs to debug comp status better
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

- Test update

#### Description
Need more logs to see component status logic.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 20:01:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/250" class=".btn">#250</a>
            </td>
            <td>
                <b>
                    Fix unjoin system channel
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
- the unjoin button from the system channel was not being shown, it now shows
- the ignore delete warnings was not be shown on orderers that used a system channel, it now shows on all orderers


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 19:11:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    fix get-channels logic if response is empty
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

- fixes the response to get-osn-channels when there are 0 channels. makes it an empty array instead of null.
- fixes `system_channel_id` filed being set to null, should be empty string when there is no system channel


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 14:47:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/248" class=".btn">#248</a>
            </td>
            <td>
                <b>
                    Updated test case to create orderer with system channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ketul Shah <shah.ketul@ibm.com>

#### Type of change
- Test update

#### Description
Updated test case to create orderer with system channel
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-07 13:18:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/247" class=".btn">#247</a>
            </td>
            <td>
                <b>
                    add the consenters to review step of create channel wizard
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

- New feature

#### Description
- show the consenter node ids in the review panel of the create channel wizard.
- surface block parsing or getting errors in join osn wizard


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 21:00:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/246" class=".btn">#246</a>
            </td>
            <td>
                <b>
                    added the system channel removal doc
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
added the system channel removal doc


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 20:02:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/245" class=".btn">#245</a>
            </td>
            <td>
                <b>
                    Fix systemless detection
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
- Fix the with or without system channel detection in the orderer details page
- Adds orderer type to side panel in orderer details page
- Fix the loading logic in the orderer details page
- Updates the node's `systemless` field after removing system channel

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 18:49:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/244" class=".btn">#244</a>
            </td>
            <td>
                <b>
                    fix title bar on login page
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
The browser's title bar on the login page was not always correct


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 20:51:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/243" class=".btn">#243</a>
            </td>
            <td>
                <b>
                    only join selected orderers to channel
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
Only join the orderers that were checked to the channel


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 20:10:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/242" class=".btn">#242</a>
            </td>
            <td>
                <b>
                    improve warning msg and fix os details tab logic
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
- Improves the "TLS identity not found" warning message on the orderer cluster details page. adds why this message is appearing and how to fix it
- Fixes logic on the orderer cluster details page showing the wrong content


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 19:59:35 +0000 UTC
    </div>
</div>

