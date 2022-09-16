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
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3374" class=".btn">#3374</a>
            </td>
            <td>
                <b>
                    fix: Docker warning when using frapsoft/openssl on arm64 system
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolved a warning from Docker that would get printed when running the generate-test-keys Makefile target on an arm64 system. The warning from Docker alerts you that the image for frapsoft/openssl is for amd64, which doesn't match the system you're on (when using an arm64-based OS). To resolve the warning, you have to either use an image that matches the system architecture, or explicitly state the platform using the --platform flag. In this case, there is only an amd64 version of frapsoft/openssl, so I added the explicit flag to resolve the warning. I also added a TODO for us to find an arm64 alternative in the future (although the amd64 version of frapsoft/openssl does seem to work fine on arm64 Mac OS currently, presumably due to Apple's Rosetta translation layer or some other emulation layer).

Signed-off-by: Derek Trider <Derek.Trider@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-15 20:44:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3372" class=".btn">#3372</a>
            </td>
            <td>
                <b>
                    feat: Validate did configuration for did and domain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Parse and validate DID configuration bytes.
Search through domain linkage credential(s) for specified did and domain. 
Validate domain linkage credential for Linked Data (JWT validation will be handled in different issue).

Closes #3371

Signed-off-by: Sandra Vrtikapa <sandra.vrtikapa@securekey.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-13 19:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3369" class=".btn">#3369</a>
            </td>
            <td>
                <b>
                    refactor: Add handling inbound problem report messages inside legacy-connection protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Problem report inside legacy connection

**Summary:**
- Add handling problem report messages inside protocol
-  Cover with unit tests


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 06:57:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3368" class=".btn">#3368</a>
            </td>
            <td>
                <b>
                    feat: fix format filtering in pEx V2 for JWTVCs, and add bdd tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - also fix an issue with initializing sdk agents, when old clients
  still exist under the same name
- also rename wallet-jsonld bdd tests since they aren't jsonld-only

Signed-off-by: Filip Burlacu <filip.burlacu@securekey.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 22:24:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3366" class=".btn">#3366</a>
            </td>
            <td>
                <b>
                    chore(deps): bump actions/upload-artifact from 2.2.4 to 3.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 2.2.4 to 3.1.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/upload-artifact/releases">actions/upload-artifact's releases</a>.</em></p>
<blockquote>
<h2>v3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump <code>@​actions/artifact</code> to v1.1.0 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/pull/327">actions/upload-artifact#327</a>)
<ul>
<li>Adds checksum headers on artifact upload (<a href="https://github-redirect.dependabot.com/actions/toolkit/pull/1095">actions/toolkit#1095</a>) (<a href="https://github-redirect.dependabot.com/actions/toolkit/pull/1063">actions/toolkit#1063</a>)</li>
</ul>
</li>
</ul>
<h2>v3.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update default runtime to node16 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/293">#293</a>)</li>
<li>Update package-lock.json file version to 2 (<a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/302">#302</a>)</li>
</ul>
<h3>Breaking Changes</h3>
<p>With the update to Node 16, all scripts will now be run with Node 16 rather than Node 12.</p>
<h2>v2.3.1</h2>
<p>Fix for empty fails on Windows failing on upload <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/281">#281</a></p>
<h2>v2.3.0 Upload Artifact</h2>
<ul>
<li>Optimizations for faster uploads of larger files that are already compressed</li>
<li>Significantly improved logging when there are chunked uploads</li>
<li>Clarifications in logs around the upload size and prohibited characters that aren't allowed in the artifact name or any uploaded files</li>
<li>Various other small bugfixes &amp; optimizations</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/upload-artifact/commit/3cea5372237819ed00197afe530f5a7ea3e805c8"><code>3cea537</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/327">#327</a> from actions/robherley/artifact-1.1.0</li>
<li><a href="https://github.com/actions/upload-artifact/commit/849aa7758a428ee22be38de371b49c8bd57c4b9d"><code>849aa77</code></a> nvm use 12 &amp; npm run release</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4d3986961d0423ba9a593efb490a2960eb65f43b"><code>4d39869</code></a> recompile with correct ncc version</li>
<li><a href="https://github.com/actions/upload-artifact/commit/2e0d362ec5cf81e334dda822c49c96dcd4b7df2c"><code>2e0d362</code></a> bump <code>@​actions/artifact</code> to 1.1.0</li>
<li><a href="https://github.com/actions/upload-artifact/commit/09a5d6a283da3e7c9f3253a5d4cdab2347712a66"><code>09a5d6a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/320">#320</a> from actions/dependabot/npm_and_yarn/ansi-regex-4.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/189315d9106f43a2a8eb60836608bb96b1f69d77"><code>189315d</code></a> Bump ansi-regex from 4.1.0 to 4.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/d159c2d80bf32e77611286e4d71bfe6d15208d88"><code>d159c2d</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/297">#297</a> from actions/dependabot/npm_and_yarn/ajv-6.12.6</li>
<li><a href="https://github.com/actions/upload-artifact/commit/c26a7ba4b5dbaecea906fec3b7d2c0c86f1ccaba"><code>c26a7ba</code></a> Bump ajv from 6.11.0 to 6.12.6</li>
<li><a href="https://github.com/actions/upload-artifact/commit/6ed6c729229a623bcb1fdd75903dc6e436b3d0a7"><code>6ed6c72</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/actions/upload-artifact/issues/303">#303</a> from actions/dependabot/npm_and_yarn/yargs-parser-13.1.2</li>
<li><a href="https://github.com/actions/upload-artifact/commit/2aeee267b2cb1f938c861a763b9770ee6e921dc3"><code>2aeee26</code></a> Bump yargs-parser from 13.1.1 to 13.1.2</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v2.2.4...v3.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/upload-artifact&package-manager=github_actions&previous-version=2.2.4&new-version=3.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 08:16:02 +0000 UTC
    </div>
</div>

