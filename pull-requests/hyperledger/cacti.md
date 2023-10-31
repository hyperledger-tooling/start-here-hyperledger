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
                PR <a href="https://github.com/hyperledger/cacti/pull/2832" class=".btn">#2832</a>
            </td>
            <td>
                <b>
                    build(deps): bump werkzeug from 2.3.6 to 3.0.1 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [werkzeug](https://github.com/pallets/werkzeug) from 2.3.6 to 3.0.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/werkzeug/releases">werkzeug's releases</a>.</em></p>
<blockquote>
<h2>3.0.1</h2>
<p>This is a security release for the 3.0.x feature branch.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/3.0.x/changes/#version-3-0-1">https://werkzeug.palletsprojects.com/en/3.0.x/changes/#version-3-0-1</a></li>
</ul>
<h2>3.0.0</h2>
<p>This is a feature release, which includes new features, removes previously deprecated code, and adds new deprecations. The 3.0.x branch is now the supported fix branch, the 2.3.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades. Test with warnings treated as errors to be able to adapt to deprecation warnings early.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/3.0.x/changes/#version-3-0-0">https://werkzeug.palletsprojects.com/en/3.0.x/changes/#version-3-0-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/21?closed=1">https://github.com/pallets/werkzeug/milestone/21?closed=1</a></li>
</ul>
<h2>2.3.7</h2>
<p>This is a fix release for the 2.3.x feature branch.</p>
<ul>
<li>Changes: <a href="https://werkzeug.palletsprojects.com/en/2.3.x/changes/#version-2-3-7">https://werkzeug.palletsprojects.com/en/2.3.x/changes/#version-2-3-7</a></li>
<li>Milestone: <a href="https://github.com/pallets/werkzeug/milestone/33?closed=1">https://github.com/pallets/werkzeug/milestone/33?closed=1</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/werkzeug/blob/main/CHANGES.rst">werkzeug's changelog</a>.</em></p>
<blockquote>
<h2>Version 3.0.1</h2>
<p>Released 2023-10-24</p>
<ul>
<li>Fix slow multipart parsing for large parts potentially enabling DoS
attacks. :cwe:<code>CWE-407</code></li>
</ul>
<h2>Version 3.0.0</h2>
<p>Released 2023-09-30</p>
<ul>
<li>Remove previously deprecated code. :pr:<code>2768</code></li>
<li>Deprecate the <code>__version__</code> attribute. Use feature detection, or
<code>importlib.metadata.version(&quot;werkzeug&quot;)</code>, instead. :issue:<code>2770</code></li>
<li><code>generate_password_hash</code> uses scrypt by default. :issue:<code>2769</code></li>
<li>Add the <code>&quot;werkzeug.profiler&quot;</code> item to the  WSGI <code>environ</code> dictionary
passed to <code>ProfilerMiddleware</code>'s <code>filename_format</code> function. It contains
the <code>elapsed</code> and <code>time</code> values for the profiled request. :issue:<code>2775</code></li>
<li>Explicitly marked the PathConverter as non path isolating. :pr:<code>2784</code></li>
</ul>
<h2>Version 2.3.8</h2>
<p>Unreleased</p>
<h2>Version 2.3.7</h2>
<p>Released 2023-08-14</p>
<ul>
<li>Use <code>flit_core</code> instead of <code>setuptools</code> as build backend.</li>
<li>Fix parsing of multipart bodies. :issue:<code>2734</code> Adjust index of last newline
in data start. :issue:<code>2761</code></li>
<li>Parsing ints from header values strips spacing first. :issue:<code>2734</code></li>
<li>Fix empty file streaming when testing. :issue:<code>2740</code></li>
<li>Clearer error message when URL rule does not start with slash. :pr:<code>2750</code></li>
<li><code>Accept</code> <code>q</code> value can be a float without a decimal part. :issue:<code>2751</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/werkzeug/commit/ce4eff5902d4a6b41a20ecc6e4029741284a87fd"><code>ce4eff5</code></a> Release version 3.0.1</li>
<li><a href="https://github.com/pallets/werkzeug/commit/b1916c0c083e0be1c9d887ee2f3d696922bfc5c1"><code>b1916c0</code></a> Fix: slow multipart parsing for huge files with few CR/LF characters</li>
<li><a href="https://github.com/pallets/werkzeug/commit/726eaa28593d859548da3477859c914732f012ef"><code>726eaa2</code></a> Release version 3.0.0</li>
<li><a href="https://github.com/pallets/werkzeug/commit/64275425888b6ca4f5ebdfa1a9df814317718290"><code>6427542</code></a> Default the PathConverter (and descendants) to be non part isolating</li>
<li><a href="https://github.com/pallets/werkzeug/commit/4820d8c487e5db9f43645c31c4123fce5ac5ad32"><code>4820d8c</code></a> Provide elapsed and timestamp info to filename_format</li>
<li><a href="https://github.com/pallets/werkzeug/commit/599993d7382eeb96add9f38b4431a2f50cd2c9f2"><code>599993d</code></a> Bump pypa/gh-action-pypi-publish from 1.8.8 to 1.8.10 (<a href="https://redirect.github.com/pallets/werkzeug/issues/2780">#2780</a>)</li>
<li><a href="https://github.com/pallets/werkzeug/commit/a2394ed51ed8697b5523243acb10cb589c0f7834"><code>a2394ed</code></a> Bump slsa-framework/slsa-github-generator from 1.7.0 to 1.9.0 (<a href="https://redirect.github.com/pallets/werkzeug/issues/2779">#2779</a>)</li>
<li><a href="https://github.com/pallets/werkzeug/commit/1efd6f3c2c31ec9479d8b8d9219bdb042e55bd15"><code>1efd6f3</code></a> Bump actions/checkout from 3.5.3 to 3.6.0 (<a href="https://redirect.github.com/pallets/werkzeug/issues/2778">#2778</a>)</li>
<li><a href="https://github.com/pallets/werkzeug/commit/76a5419d2ee8b7785c0304d58a94d6c0387c976c"><code>76a5419</code></a> Bump pypa/gh-action-pypi-publish from 1.8.8 to 1.8.10</li>
<li><a href="https://github.com/pallets/werkzeug/commit/ce8cfe7dbb73b56c982a9c74162084cdb284c2f5"><code>ce8cfe7</code></a> Bump slsa-framework/slsa-github-generator from 1.7.0 to 1.9.0</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/werkzeug/compare/2.3.6...3.0.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=werkzeug&package-manager=pip&previous-version=2.3.6&new-version=3.0.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-10-25 19:52:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2831" class=".btn">#2831</a>
            </td>
            <td>
                <b>
                    fix(connector-besu): toBuffer only supports 0x-prefixed hex
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Commit to be reviewed
---------------

fix(connector-besu): toBuffer only supports 0x-prefixed hex

```
Primary Changes
---------------
1. Updated private-deploy-contract-from-json-web3-eea.test.ts gaslimit from
3000000 to its hex equivalent
```

fixes: #2791

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
        Created At 2023-10-25 03:45:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2830" class=".btn">#2830</a>
            </td>
            <td>
                <b>
                    build(deps): bulk fix CVEs via dependency resolution overrides 2023-10-23
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                1. Couldn't get rid of vulnerable versions in a couple of dependencies
because the underlying dependencies have gone ESM only which is a blocker
for us at the moment unfortunately.
2. Swapped out the ubiquity TS client to a version of it that I self
published onto npm after a full renovation of all of its dependencies.

Depends on #2807 (because that one also has a couple of dependency bumps
that are needed to eliminate the vulnerabilities)

Fixes #2828
Fixes #2544

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
        Created At 2023-10-24 21:11:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2829" class=".btn">#2829</a>
            </td>
            <td>
                <b>
                    build(deps): replace ipfs-http-client with kubo-rpc-client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Replace deprecated ipfs-http-client with kubo-rpc-client.
- kubo-rpc-client must be imported dynamically since it's ESM-only and we still use CJS.

Depends on: #2821

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-24 11:58:50 +0000 UTC
    </div>
</div>

