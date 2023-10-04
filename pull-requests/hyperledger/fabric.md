---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4462" class=".btn">#4462</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 1.26.16 to 1.26.17
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patchset resolves the security alert of Cookie HTTP header handling.

Change-Id: I7015258f8eef9518ec7a7428d51b192aa0192b1a

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

More details can be found at
https://github.com/advisories/GHSA-v845-jxx5-vc9f.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 17:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4461" class=".btn">#4461</a>
            </td>
            <td>
                <b>
                    Improve error msg by using the error pkg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset improves the error message.

Change-Id: I7d7bb084d0ba9d6d33a2b583a763752fca530b9b

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The errors package has better features than the fmt package in terms of error processing. E.g., errors.Errorf records the stack trace at the point it is called.

On the other hand, the patchset eliminates the usage of fmt package.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 17:22:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4460" class=".btn">#4460</a>
            </td>
            <td>
                <b>
                    Tag docker images with release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When calling "make docker", tag the images with the Fabric version and Fabric two-digit version number. This will ensure that the correct ccenv and baseos images can be found when building chaincode images.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 15:03:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4458" class=".btn">#4458</a>
            </td>
            <td>
                <b>
                    Expose block censorship timeout in config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code)
- Test update

#### Description

As described in issue #4401 

#### Related issues

issue #4401 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 09:14:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4457" class=".btn">#4457</a>
            </td>
            <td>
                <b>
                    Bump urllib3 from 1.26.16 to 1.26.17 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [urllib3](https://github.com/urllib3/urllib3) from 1.26.16 to 1.26.17.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/releases">urllib3's releases</a>.</em></p>
<blockquote>
<h2>1.26.17</h2>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (GHSA-v845-jxx5-vc9f)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/urllib3/urllib3/blob/main/CHANGES.rst">urllib3's changelog</a>.</em></p>
<blockquote>
<h1>1.26.17 (2023-10-02)</h1>
<ul>
<li>Added the <code>Cookie</code> header to the list of headers to strip from requests when redirecting to a different host. As before, different headers can be set via <code>Retry.remove_headers_on_redirect</code>. (<code>[#3139](https://github.com/urllib3/urllib3/issues/3139) &lt;https://github.com/urllib3/urllib3/pull/3139&gt;</code>_)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/urllib3/urllib3/commit/c9016bf464751a02b7e46f8b86504f47d4238784"><code>c9016bf</code></a> Release 1.26.17</li>
<li><a href="https://github.com/urllib3/urllib3/commit/01220354d389cd05474713f8c982d05c9b17aafb"><code>0122035</code></a> Backport GHSA-v845-jxx5-vc9f (<a href="https://redirect.github.com/urllib3/urllib3/issues/3139">#3139</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/e63989f97d206e839ab9170c8a76e3e097cc60e8"><code>e63989f</code></a> Fix installing <code>brotli</code> extra on Python 2.7</li>
<li><a href="https://github.com/urllib3/urllib3/commit/2e7a24d08713a0131f0b3c7197889466d645cc49"><code>2e7a24d</code></a> [1.26] Configure OS for RTD to fix building docs</li>
<li><a href="https://github.com/urllib3/urllib3/commit/57181d6ea910ac7cb2ff83345d9e5e0eb816a0d0"><code>57181d6</code></a> [1.26] Improve error message when calling urllib3.request() (<a href="https://redirect.github.com/urllib3/urllib3/issues/3058">#3058</a>)</li>
<li><a href="https://github.com/urllib3/urllib3/commit/3c0148048a523325819377b23fc67f8d46afc3aa"><code>3c01480</code></a> [1.26] Run coverage even with failed jobs</li>
<li>See full diff in <a href="https://github.com/urllib3/urllib3/compare/1.26.16...1.26.17">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=urllib3&package-manager=pip&previous-version=1.26.16&new-version=1.26.17)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-03 04:00:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4455" class=".btn">#4455</a>
            </td>
            <td>
                <b>
                    BFT: orderer deliver headers on cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix
- New feature

#### Description

The orderer delivers blocks with  block.Data=nil when asked for SeekInfo_HEADER_WITH_SIG. However, one needs to avoid mutating the block received from the block iterator, as those are from a cache.

#### Related issues

#4456
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 14:42:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4454" class=".btn">#4454</a>
            </td>
            <td>
                <b>
                    Extend _lifecycle functions on checkcommitreadiness to provide detail of the discrepancies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch updates some _lifecycle functions on checkcommitreadiness to provide details of the discrepancies.

#### Type of change

- New feature

#### Description

I have proposed an extension to lifecycle chaincode checkcommitreadiness to provide details of the discrepancies as shown in  https://github.com/hyperledger/fabric/issues/4428.

As a sub-task stemming from issue #4428, this patch updates some _lifecycle functions on checkcommitreadiness to provide details of the discrepancies.

Once this patch is merged, I will submit the following commit to enhance the command:
- https://github.com/satota2/fabric/commit/9ea8ad11de451139af61cf73281feff656a38d07

#### Additional details

The example of output when executing checkcommitreadiness with inspect flag in the provisional implementation:

```
peer lifecycle chaincode checkcommitreadiness --channelID mychannel --name basic --version 2.0 --sequence 2 --inspect
Chaincode definition for chaincode 'basic', version '2.0', sequence '2' on channel 'mychannel' approval status by org:
Org1MSP: false (mismatch: [EndorsementInfo, ValidationInfo, Collections])
Org2MSP: false (mismatch: [ChaincodeParameters])
```

```
peer lifecycle chaincode checkcommitreadiness --channelID mychannel --name basic --version 2.0 --sequence 2 --inspect --output json
{
        "approvals": {
                "Org1MSP": false,
                "Org2MSP": false
        },
        "mismatches": {
                "Org1MSP": {
                        "items": [
                                "EndorsementInfo (Check the Version, InitRequired, EndorsementPlugin)",
                                "ValidationInfo (Check the ValidationParameter, ValidationPlugin)",
                                "Collections (Check the Collections)"
                        ]
                },
                "Org2MSP": {
                        "items": [
                                "ChaincodeParameters (Check the Sequence, ChaincodeName)"
                        ]
                }
        }
}
```

#### Releated Issues

- https://github.com/hyperledger/fabric/issues/4428


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-02 08:32:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4453" class=".btn">#4453</a>
            </td>
            <td>
                <b>
                    Add error check and improve msg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset checks the error when doing yaml marshal, and improves the message when error happens.

Change-Id: I40fb7dbe930bcdc6563078daab50f4f4564c3381

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

* Check the possible error in marshaling;
* Improve message when error happens.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 17:08:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4452" class=".btn">#4452</a>
            </td>
            <td>
                <b>
                    Simplify code structure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset simplify the code structure by following Go style.

Change-Id: I47ef0605e17fd4c16a51cd104b8c90d247ce03f7

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

* Use the switch structure;
* Use the error checking directly.

#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 16:54:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4451" class=".btn">#4451</a>
            </td>
            <td>
                <b>
                    Update pluggable_endorsement_and_validation.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #2814

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

Node SDK no longer supports chaincode deployment, and therefore the referenced doc page doesn't exist anymore. In this case the entire following sentence should be deleted.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-29 10:05:02 +0000 UTC
    </div>
</div>

