---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1146" class=".btn">#1146</a>
            </td>
            <td>
                <b>
                    fix: expose AttachmentData and DiscoverFeaturesEvents
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Expose AttachmentData and Discover Features events... and some minor housekeeping to remove a few lint warnings.

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 21:27:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1143" class=".btn">#1143</a>
            </td>
            <td>
                <b>
                    feat: remove keys on mediator when deleting connections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses the case where a mobile agent (or any agent that uses mediator) deletes a connection or OOB record, meaning that the corresponding recipient keys should be removed from its mediator (as per [Aries RFC 0211](https://github.com/hyperledger/aries-rfcs/blob/main/features/0211-route-coordination/README.md)). Otherwise, mediator will still be forwarding messages to the agent that can't (and more importantly _don't want to_) be handled.

This will mean that, when using mediator, in order to delete a connection or out-of-band record, the agent must be online. This is aligned to the opposite case: connection and OOB invitation creation, which also need the agent to be online to be in sync with its mediator.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 03:11:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1141" class=".btn">#1141</a>
            </td>
            <td>
                <b>
                    feat: Support for DIDCommV2 mediator provisioning and related protocols
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains changes adding support for DIDCommV2 based mediator provisioning and pickup / routing protocols and also depends on [PR which contains general DidComm V2 support](https://github.com/hyperledger/aries-framework-javascript/pull/1096) and must be merged first


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 11:30:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1140" class=".btn">#1140</a>
            </td>
            <td>
                <b>
                    refactor: simplify acceptXXX methods and jsonld format service interfaces should take JSON credential instead of instance of W3cCredential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR covers three issues: 

#1089 (Part 1)
#1126 
#1132 


I closed the previous PR related to 1089 as I discovered dependencies between it and #1126) so it made more sense to package them up together in one PR
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-05 09:49:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1139" class=".btn">#1139</a>
            </td>
            <td>
                <b>
                    build(deps): bump decode-uri-component from 0.2.0 to 0.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [decode-uri-component](https://github.com/SamVerschueren/decode-uri-component) from 0.2.0 to 0.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/SamVerschueren/decode-uri-component/releases">decode-uri-component's releases</a>.</em></p>
<blockquote>
<h2>v0.2.2</h2>
<ul>
<li>Prevent overwriting previously decoded tokens  980e0bf</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.1...v0.2.2</a></p>
<h2>v0.2.1</h2>
<ul>
<li>Switch to GitHub workflows  76abc93</li>
<li>Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a>  746ca5d</li>
<li>Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)  486d7e2</li>
<li>Tidelift tasks  a650457</li>
<li>Meta tweaks  66e1c28</li>
</ul>
<p><a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1">https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.1</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a0eea469d26eb0df668b081672cdb9581feb78eb"><code>a0eea46</code></a> 0.2.2</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/980e0bf09b64d94f1aa79012f895816c30ffd152"><code>980e0bf</code></a> Prevent overwriting previously decoded tokens</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/3c8a373dd4837e89b3f970e01295dd03e1405a33"><code>3c8a373</code></a> 0.2.1</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/76abc939783fe3900fadb7d384a74d324d5557f3"><code>76abc93</code></a> Switch to GitHub workflows</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/746ca5dcb6667c5d364e782d53c542830e4c10b9"><code>746ca5d</code></a> Fix issue where decode throws - fixes <a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/6">#6</a></li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/486d7e26d3a8c0fbe860fb651fe1bc98c2f2be30"><code>486d7e2</code></a> Update license (<a href="https://github-redirect.dependabot.com/SamVerschueren/decode-uri-component/issues/1">#1</a>)</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/a65045724e6234acef87f31da499d4807b20b134"><code>a650457</code></a> Tidelift tasks</li>
<li><a href="https://github.com/SamVerschueren/decode-uri-component/commit/66e1c2834c0e189201cb65196ec3101372459b02"><code>66e1c28</code></a> Meta tweaks</li>
<li>See full diff in <a href="https://github.com/SamVerschueren/decode-uri-component/compare/v0.2.0...v0.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=decode-uri-component&package-manager=npm_and_yarn&previous-version=0.2.0&new-version=0.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-04 22:34:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    refactor(oob)!: merge oob invitation parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BREAKING CHANGE: the `agent.oob.parseInvitationShortUrl` method has been removed and integrated with the `agent.oob.parseInvitationUrl`. Because of this, the `agent.oob.parseInvitationUrl` method is now asynchronous.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-01 11:37:30 +0000 UTC
    </div>
</div>

