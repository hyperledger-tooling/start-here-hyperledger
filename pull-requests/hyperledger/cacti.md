---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3027" class=".btn">#3027</a>
            </td>
            <td>
                <b>
                    build(deps): bump undici from 5.26.2 to 5.28.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [undici](https://github.com/nodejs/undici) from 5.26.2 to 5.28.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/nodejs/undici/releases">undici's releases</a>.</em></p>
<blockquote>
<h2>v5.28.3</h2>
<h2>⚠️ Security Release ⚠️</h2>
<p>Fixes:</p>
<ul>
<li><a href="https://github.com/nodejs/undici/security/advisories/GHSA-3787-6prv-h9w3">CVE-2024-24758 Proxy-Authorization header not cleared on cross-origin redirect in fetch</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.28.2...v5.28.3">https://github.com/nodejs/undici/compare/v5.28.2...v5.28.3</a></p>
<h2>v5.28.2</h2>
<h2>What's Changed</h2>
<ul>
<li>fix: remove optional chainning for compatible with Nodejs12 and below by <a href="https://github.com/bugb"><code>@​bugb</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2470">nodejs/undici#2470</a></li>
<li>fix: remove <code>node:</code> prefix by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2471">nodejs/undici#2471</a></li>
<li>perf: avoid Headers initialization by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2468">nodejs/undici#2468</a></li>
<li>fix: handle SharedArrayBuffer correctly by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2466">nodejs/undici#2466</a></li>
<li>fix: Add <code>null</code> type to <code>signal</code> in <code>RequestInit</code> by <a href="https://github.com/gebsh"><code>@​gebsh</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2455">nodejs/undici#2455</a></li>
<li>fix: correctly handle data URL with hashes. by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2475">nodejs/undici#2475</a></li>
<li>fix: check response for timinginfo allow flag by <a href="https://github.com/ToshB"><code>@​ToshB</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2477">nodejs/undici#2477</a></li>
<li>Make call to onBodySent conditional in RetryHandler by <a href="https://github.com/MzUgM"><code>@​MzUgM</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2478">nodejs/undici#2478</a></li>
<li>refactor: better integrity check by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2462">nodejs/undici#2462</a></li>
<li>fix: Added support for inline URL username:password proxy auth by <a href="https://github.com/matt-way"><code>@​matt-way</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2473">nodejs/undici#2473</a></li>
<li>build(deps-dev): bump jsdom from 22.1.0 to 23.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2472">nodejs/undici#2472</a></li>
<li>build(deps-dev): bump sinon from 16.1.3 to 17.0.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2405">nodejs/undici#2405</a></li>
<li>build(deps): bump ossf/scorecard-action from 2.2.0 to 2.3.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2396">nodejs/undici#2396</a></li>
<li>build(deps): bump actions/setup-node from 3.8.1 to 4.0.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2395">nodejs/undici#2395</a></li>
<li>build(deps): bump step-security/harden-runner from 2.5.0 to 2.6.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2392">nodejs/undici#2392</a></li>
<li>build(deps-dev): bump formdata-node from 4.4.1 to 6.0.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2389">nodejs/undici#2389</a></li>
<li>build(deps): bump actions/upload-artifact from 3.1.2 to 3.1.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2302">nodejs/undici#2302</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/bugb"><code>@​bugb</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2470">nodejs/undici#2470</a></li>
<li><a href="https://github.com/gebsh"><code>@​gebsh</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2455">nodejs/undici#2455</a></li>
<li><a href="https://github.com/ToshB"><code>@​ToshB</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2477">nodejs/undici#2477</a></li>
<li><a href="https://github.com/MzUgM"><code>@​MzUgM</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2478">nodejs/undici#2478</a></li>
<li><a href="https://github.com/matt-way"><code>@​matt-way</code></a> made their first contribution in <a href="https://redirect.github.com/nodejs/undici/pull/2473">nodejs/undici#2473</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.28.1...v5.28.2">https://github.com/nodejs/undici/compare/v5.28.1...v5.28.2</a></p>
<h2>v5.28.1</h2>
<h2>What's Changed</h2>
<ul>
<li>perf: Improve <code>normalizeMethod</code> by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2456">nodejs/undici#2456</a></li>
<li>fix: dispatch error handling by <a href="https://github.com/ronag"><code>@​ronag</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2459">nodejs/undici#2459</a></li>
<li>perf(request): optimize if headers are given by <a href="https://github.com/tsctx"><code>@​tsctx</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2454">nodejs/undici#2454</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/nodejs/undici/compare/v5.28.0...v5.28.1">https://github.com/nodejs/undici/compare/v5.28.0...v5.28.1</a></p>
<h2>v5.28.0</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(parseHeaders): util.parseHeaders handle correctly array of buffer… by <a href="https://github.com/mdoria12"><code>@​mdoria12</code></a> in <a href="https://redirect.github.com/nodejs/undici/pull/2398">nodejs/undici#2398</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/nodejs/undici/commit/e71cb4c88faae5670a129fde5552266afc2dbc39"><code>e71cb4c</code></a> Bumped v5.28.3</li>
<li><a href="https://github.com/nodejs/undici/commit/20c65b89f4fda588ebb3f2abf51c55726880820e"><code>20c65b8</code></a> Fix tests for Node.js v20.11.0 (<a href="https://redirect.github.com/nodejs/undici/issues/2618">#2618</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/8ec52cde66e288ea98f9f801c29e6e845bf4c5f1"><code>8ec52cd</code></a> Fix tests for Node.js v21 (<a href="https://redirect.github.com/nodejs/undici/issues/2609">#2609</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/d3aa574b1259c1d8d329a0f0f495ee82882b1458"><code>d3aa574</code></a> Merge pull request from GHSA-3787-6prv-h9w3</li>
<li><a href="https://github.com/nodejs/undici/commit/9a14e5f32a118fa93e769cc15ae8de9de552f2e4"><code>9a14e5f</code></a> Bumped v5.28.2</li>
<li><a href="https://github.com/nodejs/undici/commit/fcdfe878d792c4347b81179bc31a2d1b1f06e8fb"><code>fcdfe87</code></a> build(deps): bump actions/upload-artifact from 3.1.2 to 3.1.3 (<a href="https://redirect.github.com/nodejs/undici/issues/2302">#2302</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/169c157f9a576e4422a20060f57db1dc4693b373"><code>169c157</code></a> build(deps-dev): bump formdata-node from 4.4.1 to 6.0.3 (<a href="https://redirect.github.com/nodejs/undici/issues/2389">#2389</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/97881779e6ba41d2fdbfe27b5c9cc0563dc60134"><code>9788177</code></a> build(deps): bump step-security/harden-runner from 2.5.0 to 2.6.0 (<a href="https://redirect.github.com/nodejs/undici/issues/2392">#2392</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/1f6d1597648d332c0705befec74387631d5df9ff"><code>1f6d159</code></a> build(deps): bump actions/setup-node from 3.8.1 to 4.0.0 (<a href="https://redirect.github.com/nodejs/undici/issues/2395">#2395</a>)</li>
<li><a href="https://github.com/nodejs/undici/commit/a393a86d09581945ce4e601d2359023e901b2dd0"><code>a393a86</code></a> build(deps): bump ossf/scorecard-action from 2.2.0 to 2.3.1 (<a href="https://redirect.github.com/nodejs/undici/issues/2396">#2396</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/nodejs/undici/compare/v5.26.2...v5.28.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=undici&package-manager=npm_and_yarn&previous-version=5.26.2&new-version=5.28.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 17:15:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3025" class=".btn">#3025</a>
            </td>
            <td>
                <b>
                    build(weaver/corda-driver): add Trivy scanning capability and steps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The build.gradle file now has the maven publish plugin pulled which
can be used to generate pom.xml files that we don't really plan on using
for publishing but are still necessary to have in a temporary fashion
because the scanning tool (Trivy) only suports scanning dependencies
for vulnerabilities via pom.xml files of the Maven tool but not through
`build.gradle` files of the Gradle tool.
2. The `README.md` file was updated with detailed steps on how to run a
scan that includes generating the pom file, renaming it according to the
requirements of Trivy itself and then running the actual scan.
3. Some of the cspell issues have been rectified by adding new words to
the config.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 22:14:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3024" class=".btn">#3024</a>
            </td>
            <td>
                <b>
                    build(devcontainer): add trivy to the image specification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This will result in the `trivy` binary being available on the path
of the dev container after a first/re-build.
2. The tool can be used to scan dependencies for versions that have
vulnerabilities.
3. The scanning has to be done a per-package basis instead of being
possible to scan the entire mono-repo in one fell swoop.
4. The documentation for the tool can be found here: https://github.com/aquasecurity/trivy

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 22:13:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3022" class=".btn">#3022</a>
            </td>
            <td>
                <b>
                    test(tools/docker): add new Corda v4.12-SNAPSHOT all-in-one image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Published on GHCR as
`ghcr.io/hyperledger/cactus-corda-4-12-all-in-one-negotiation:2024-02-13-dev`

1. It is a more bare bones flavor of the previous versions in the sense that it does not support
running the REST API web servers that come with the samples repository at all. It only supports
running the nodes A, B and Notary.
2. There is no Party C because we had to switch over to the negotiation-cordapp example.
3. This flavor of the image supports customizing the log levels of the Corda node through
the file at: tools/docker/corda-all-in-one/corda-v4_12/negotiation-cordapp/log4j2.xml
Note however that applying these changes requires a rebuild of the image so it's still less
convenient than idea lto use, but at least now we have an option to do so.
4. Another new feature of this image compared to the earlier Corda AIO images is that it
uses Ubuntu 22.04 LTS as it's base instead of alpine. This increases the image size a little
but it's well worth the trade-off of having a uniform image base (which is the long term plan)
5. There is a builder stage that can be used to clone an arbitrary branch + SHA combination of
the upstream corda git repository and then build the node .jar file from it which then will be
used by the image to run the nodes. The custom-built .jar file is placed under  /opt/bin/corda.jar
so do not mix that one up with the other one that is provided with the corda kotlin-samples repo.
6. The `run-notary-node.sh`, `run-party-a-node.sh` and `run-party-b-node.sh` scripts were altered
to use the custom-built .jar file mentioned above and this is the reason why this commit adds
a (seeming) clone of these scripts.
7. For now I did not add a CI task for building and publishing the image because even though
that would match the older images, I'm trying to save on CI resources and at the moment we
don't necessarily need a fresh build of this image on each new pull request.
8. Last but not least (first actually) this is also a security adjacent upgrade since using
this image is the precursor to a much bigger change that will see the Corda v4 connector's
dependencies upgraded to Spring Boot v3 and Corda v4.12-SNAPSHOT but we can't do that without
having this image published first if we want to have test-automation verifying those changes.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 00:22:45 +0000 UTC
    </div>
</div>

