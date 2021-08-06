---
layout: default
title: fabric-sdk-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-sdk-java
---

# fabric-sdk-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-sdk-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-sdk-java/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    [Security] Bump commons-compress from 1.20 to 1.21
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">security</span>
            </td>
            <td>
                Bumps commons-compress from 1.20 to 1.21. **This update includes security fixes.**
<details>
<summary>Vulnerabilities fixed</summary>
<p><em>Sourced from <a href="https://github.com/advisories/GHSA-xqfj-vm6h-2x34">The GitHub Security Advisory Database</a>.</em></p>
<blockquote>
<p><strong>Improper Handling of Length Parameter Inconsistency in Compress</strong>
When reading a specially crafted TAR archive, Compress can be made to allocate large amounts of memory that finally leads to an out of memory error even for very small inputs. This could be used to mount a denial of service attack against services that use Compress' tar package.</p>
<p>Affected versions: &lt; 1.21</p>
</blockquote>
<p><em>Sourced from <a href="https://github.com/advisories/GHSA-mc84-pj99-q6hh">The GitHub Security Advisory Database</a>.</em></p>
<blockquote>
<p><strong>Improper Handling of Length Parameter Inconsistency in Compress</strong>
When reading a specially crafted ZIP archive, Compress can be made to allocate large amounts of memory that finally leads to an out of memory error even for very small inputs. This could be used to mount a denial of service attack against services that use Compress' zip package.</p>
<p>Affected versions: &lt; 1.21</p>
</blockquote>
<p><em>Sourced from <a href="https://github.com/advisories/GHSA-7hfm-57qf-j43q">The GitHub Security Advisory Database</a>.</em></p>
<blockquote>
<p><strong>Excessive Iteration in Compress</strong>
When reading a specially crafted 7Z archive, the construction of the list of codecs that decompress an entry can result in an infinite loop. This could be used to mount a denial of service attack against services that use Compress' sevenz package.</p>
<p>Affected versions: &lt; 1.21</p>
</blockquote>
<p><em>Sourced from <a href="https://github.com/advisories/GHSA-crv7-7245-f45f">The GitHub Security Advisory Database</a>.</em></p>
<blockquote>
<p><strong>Improper Handling of Length Parameter Inconsistency in Compress</strong>
When reading a specially crafted 7Z archive, Compress can be made to allocate large amounts of memory that finally leads to an out of memory error even for very small inputs. This could be used to mount a denial of service attack against services that use Compress' sevenz package.</p>
<p>Affected versions: &lt; 1.21</p>
</blockquote>
</details>
<br />


[![Dependabot compatibility score](https://api.dependabot.com/badges/compatibility_score?dependency-name=org.apache.commons:commons-compress&package-manager=maven&previous-version=1.20&new-version=1.21)](https://dependabot.com/compatibility-score/?dependency-name=org.apache.commons:commons-compress&package-manager=maven&previous-version=1.20&new-version=1.21)

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
- `@dependabot badge me` will comment on this PR with code to add a "Dependabot enabled" badge to your readme

Additionally, you can set the following in your Dependabot [dashboard](https://app.dependabot.com):
- Update frequency (including time of day and day of week)
- Pull request limits (per update run and/or open at any time)
- Automerge options (never/patch/minor, and dev/runtime dependencies)
- Out-of-range updates (receive only lockfile updates, if desired)
- Security updates (receive only security updates, if desired)



</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-02 16:59:57 +0000 UTC
    </div>
</div>

