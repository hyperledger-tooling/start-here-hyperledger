---
layout: default
title: aries-acapy-controllers
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-controllers
---

# aries-acapy-controllers <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-controllers){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Bump Newtonsoft.Json from 12.0.3 to 13.0.1 in /AliceFaberAcmeDemo/controllers/faber-controller/FaberController
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">.NET</span>
            </td>
            <td>
                Bumps [Newtonsoft.Json](https://github.com/JamesNK/Newtonsoft.Json) from 12.0.3 to 13.0.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/JamesNK/Newtonsoft.Json/releases">Newtonsoft.Json's releases</a>.</em></p>
<blockquote>
<h2>13.0.1</h2>
<ul>
<li>New feature - Add JsonSelectSettings with configuration for a regex timeout</li>
<li>Change - Remove portable assemblies from NuGet package</li>
<li>Change - JsonReader and JsonSerializer MaxDepth defaults to 64</li>
<li>Fix - Fixed throwing missing member error on ignored fields</li>
<li>Fix - Fixed various nullable annotations</li>
<li>Fix - Fixed annotations not being copied when tokens are cloned</li>
<li>Fix - Fixed naming strategy not being used when deserializing dictionary enum keys</li>
<li>Fix - Fixed serializing nullable struct dictionaries</li>
<li>Fix - Fixed JsonWriter.WriteToken to allow null with string token</li>
<li>Fix - Fixed missing error when deserializing JToken with a contract type mismatch</li>
<li>Fix - Fixed JTokenWriter when writing comment to an object</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/ae9fe44e1323e91bcbd185ca1a14099fba7c021f"><code>ae9fe44</code></a> Remove compiler package and update sourcelink (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2498">#2498</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/8ef662189dd7fc890c8fcd832d3e283edb90ef31"><code>8ef6621</code></a> Remove prerelease for 13.0.1</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/11331f50fd1c09dc1f44fe17ef26aba7c460b42c"><code>11331f5</code></a> Update SDK to 5.0.200 (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2495">#2495</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/c7e8abc09de751785355e3f972150f8a72379b02"><code>c7e8abc</code></a> Update to 13.0.1-beta2</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/1745d7c14ec7e4244a5ca1c7ddf5d955cf7d1f43"><code>1745d7c</code></a> Fix JTokenWriter when writing comment to an object (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2493">#2493</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/583eb120152f8b6332df2fe3d4b9f4c947c944d0"><code>583eb12</code></a> Fix missing error when deserializing JToken with a contract type mismatch (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2">#2</a>...</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/b6dc05be5a0f4808f06ec430f3bb59b24d3fbc3e"><code>b6dc05b</code></a> Change MaxDepth default to 64 (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2473">#2473</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/15525f1c44e0d99ef8fdee73430853e22239181d"><code>15525f1</code></a> Fix JsonWriter.WriteToken to allow null with string token (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2472">#2472</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/926d2f0f42292cfcdf07cdadeb501b73fd5b1d52"><code>926d2f0</code></a> Enable embed untracked sources (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2471">#2471</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/0a56633b6cd4fccc860a8486260ee67636f3fe90"><code>0a56633</code></a> Fixes <a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2372">#2372</a> - variable typos (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2465">#2465</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/JamesNK/Newtonsoft.Json/compare/12.0.3...13.0.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=Newtonsoft.Json&package-manager=nuget&previous-version=12.0.3&new-version=13.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-controllers/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-22 23:31:58 +0000 UTC
    </div>
</div>

