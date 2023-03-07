---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3547" class=".btn">#3547</a>
            </td>
            <td>
                <b>
                    feat: PresentationDefinition API improvements:
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - CreateVP methods set VP IDs
- Match supports merged submission map[string]interface{} and VP submission fields of PresentationSubmission type.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 17:19:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3546" class=".btn">#3546</a>
            </td>
            <td>
                <b>
                    chore(deps): bump github.com/tidwall/gjson from 1.6.7 to 1.9.3 in /test/bdd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/tidwall/gjson](https://github.com/tidwall/gjson) from 1.6.7 to 1.9.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tidwall/gjson/commit/77a57fda87dca6d0d7d4627d512a630f89a91c96"><code>77a57fd</code></a> Limit the complexity of &quot;like&quot; queries that match on a pattern.</li>
<li><a href="https://github.com/tidwall/gjson/commit/590010fdac311cc8990ef5c97448d4fec8f29944"><code>590010f</code></a> Update match dependency</li>
<li><a href="https://github.com/tidwall/gjson/commit/61273bfa669f034e10e55b9e0f540039c856ac6d"><code>61273bf</code></a> Update dependency</li>
<li><a href="https://github.com/tidwall/gjson/commit/78289be4edb19b3b82f14a3559d16347823fd45e"><code>78289be</code></a> Create FUNDING.yml</li>
<li><a href="https://github.com/tidwall/gjson/commit/75046d2a7a897e7226567313883d6a4bbe33622f"><code>75046d2</code></a> Update comments</li>
<li><a href="https://github.com/tidwall/gjson/commit/5827eb3b24ecfd17b5da5d1092dd2a84946ffa9e"><code>5827eb3</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/tidwall/gjson/issues/226">#226</a> from ifraixedes/if/fix-doc-map-method</li>
<li><a href="https://github.com/tidwall/gjson/commit/807836a222395e6a124fb186453a545bda0cd88a"><code>807836a</code></a> Minor update</li>
<li><a href="https://github.com/tidwall/gjson/commit/44b8c19d87567a8e5a322277299c7b9802fb68c2"><code>44b8c19</code></a> Minor update to test</li>
<li><a href="https://github.com/tidwall/gjson/commit/160fb9d6a148f0e04addc47b1c211b161365eb72"><code>160fb9d</code></a> Updated comments</li>
<li><a href="https://github.com/tidwall/gjson/commit/52919fa7b0887a94f2d4e020af1ac4907245492e"><code>52919fa</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/tidwall/gjson/issues/222">#222</a> from sspaink/arrayindex</li>
<li>Additional commits viewable in <a href="https://github.com/tidwall/gjson/compare/v1.6.7...v1.9.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/tidwall/gjson&package-manager=go_modules&previous-version=1.6.7&new-version=1.9.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-go/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-07 03:38:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3545" class=".btn">#3545</a>
            </td>
            <td>
                <b>
                    feat: PresentationDefinition API for submitting multi-presentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-04 06:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3544" class=".btn">#3544</a>
            </td>
            <td>
                <b>
                    fix: Wallet query multi-descriptor fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If we have two input descriptors with two credentials and one descriptor is satisfied with two credentials then we have failure depending on the order of processing.

Closes #3543




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 19:38:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3542" class=".btn">#3542</a>
            </td>
            <td>
                <b>
                    wip: Add SD-JWT Docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add SD-JWT Docs


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 21:00:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3541" class=".btn">#3541</a>
            </td>
            <td>
                <b>
                    fix: pass document loader
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
        Created At 2023-03-02 14:41:18 +0000 UTC
    </div>
</div>

