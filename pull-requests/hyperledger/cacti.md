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
                PR <a href="https://github.com/hyperledger/cacti/pull/2353" class=".btn">#2353</a>
            </td>
            <td>
                <b>
                    fix(interopcc): build failing after golang.org/x/crypto bump to v0.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    Upgraded all go modules to go v1.20
    
Closes #2348 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 18:21:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2351" class=".btn">#2351</a>
            </td>
            <td>
                <b>
                    fix(relay): rust build fails after tokio bump from 0.2.25 to 1.18.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    Additionally:
    - upgrade other dependencies for relay
    - added tls based unit test in relay

Closes #2349 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 16:46:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2350" class=".btn">#2350</a>
            </td>
            <td>
                <b>
                    chore(release): publish v1.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-28 05:52:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2347" class=".btn">#2347</a>
            </td>
            <td>
                <b>
                    refactor: package name for weaver cordapps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update package name for weaver cordapps to prefix with `org.hyperledger.cacti.weaver`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 07:17:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2346" class=".btn">#2346</a>
            </td>
            <td>
                <b>
                    fix(security): upgrade express-jwt to v8.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes/changes that needed to be done in order to make the upgrade work:
1. The HTTP verbs for exempted endpoints are now specified both as lowercase and uppercase meaning that if a specific endpoint is configured to be exempt from JWT authorization then it's method will be specified twice, once as 'POST' and once as 'post' because the underlying library (which is called express-unless) does not have the ability to handle verbs in a case insensitive way.

2. In the registerWebServiceEndpoint function, the configuration of the express-jwt-authz library had to be changed because the scope enforcement was broken due to express-jwt changing the default request property where it places the decoded JWT payload from `"user"` to `"auth"` and this made it incompatible by default with the behavior of express-jwt-authz Luckily there is a parameter to set the request property name and that is now being specified explicitly as `"auth"` so that they are playing nice with each other once again and the authorization's scope based access control works just fine.

Fixes #2231
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-25 03:57:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2345" class=".btn">#2345</a>
            </td>
            <td>
                <b>
                    build(deps): bump openssl from 0.10.41 to 0.10.48 in /weaver/core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.41 to 0.10.48.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl v0.10.48</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix LibreSSL version checking in openssl/ by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1851">sfackler/rust-openssl#1851</a></li>
<li>Skip a test that hangs on OpenSSL 3.1.0 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1850">sfackler/rust-openssl#1850</a></li>
<li>Improve reliability of some tests by <a href="https://github.com/smoelius"><code>@​smoelius</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1852">sfackler/rust-openssl#1852</a></li>
<li>Fix a series of security issues by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1854">sfackler/rust-openssl#1854</a></li>
<li>Release openssl v0.10.48 and openssl-sys v0.9.83 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1855">sfackler/rust-openssl#1855</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/smoelius"><code>@​smoelius</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1852">sfackler/rust-openssl#1852</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.47...openssl-v0.10.48">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.47...openssl-v0.10.48</a></p>
<h2>openssl v0.10.47</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.46</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.45</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.44</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.43</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.42</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4ff734fe4c5a22f7346b7b3c47ece4c4c1c01817"><code>4ff734f</code></a> Release openssl v0.10.48 and openssl-sys v0.9.83 (<a href="https://redirect.github.com/sfackler/rust-openssl/issues/1855">#1855</a>)</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/5efceaabd69c540b487f6372be4982cf94884008"><code>5efceaa</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1854">#1854</a> from alex/davids-openssl-of-horrors</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/6ced4f305e44df7ca32e478621bf4840b122f1a3"><code>6ced4f3</code></a> Fix race condition with X509Name creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a7528056c5be6f3fbabc52c2fd02882b208d5939"><code>a752805</code></a> Document the horror show</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/78aa9aa22cfd58ac33d1e19184cec667438fd2a1"><code>78aa9aa</code></a> Always provide an X509V3Context in X509Extension::new because OpenSSL require...</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/332311b597cc444a10d4acaf122ee58bd1bc8ff8"><code>332311b</code></a> Resolve an injection vulnerability in EKU creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/482575bff434f58b80ffea34a9610d0ff265ac1f"><code>482575b</code></a> Resolve an injection vulnerability in SAN creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/690eeb2ac20d47e43f04d8cb43f03d4128946b81"><code>690eeb2</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1852">#1852</a> from smoelius/master</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/e5b6d97ed170f835b56440d79edcd46381a46ebc"><code>e5b6d97</code></a> Improve reliability of some tests</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/319200ab93e252a3c0e127adc1e4c43a90f063a1"><code>319200a</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1851">#1851</a> from alex/libressl-versions</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.41...openssl-v0.10.48">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.41&new-version=0.10.48)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-25 00:57:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2344" class=".btn">#2344</a>
            </td>
            <td>
                <b>
                    build(deps): bump openssl from 0.10.32 to 0.10.48 in /packages/cactus-plugin-keychain-vault/src/cactus-keychain-vault-server/rust/gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.32 to 0.10.48.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl v0.10.48</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix LibreSSL version checking in openssl/ by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1851">sfackler/rust-openssl#1851</a></li>
<li>Skip a test that hangs on OpenSSL 3.1.0 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1850">sfackler/rust-openssl#1850</a></li>
<li>Improve reliability of some tests by <a href="https://github.com/smoelius"><code>@​smoelius</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1852">sfackler/rust-openssl#1852</a></li>
<li>Fix a series of security issues by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1854">sfackler/rust-openssl#1854</a></li>
<li>Release openssl v0.10.48 and openssl-sys v0.9.83 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1855">sfackler/rust-openssl#1855</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/smoelius"><code>@​smoelius</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/1852">sfackler/rust-openssl#1852</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.47...openssl-v0.10.48">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.47...openssl-v0.10.48</a></p>
<h2>openssl v0.10.47</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.46</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.45</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.44</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.43</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.42</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.41</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.40</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.39</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.38</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.37</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.36</h2>
<p>No release notes provided.</p>
<h2>openssl v0.10.35</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4ff734fe4c5a22f7346b7b3c47ece4c4c1c01817"><code>4ff734f</code></a> Release openssl v0.10.48 and openssl-sys v0.9.83 (<a href="https://redirect.github.com/sfackler/rust-openssl/issues/1855">#1855</a>)</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/5efceaabd69c540b487f6372be4982cf94884008"><code>5efceaa</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1854">#1854</a> from alex/davids-openssl-of-horrors</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/6ced4f305e44df7ca32e478621bf4840b122f1a3"><code>6ced4f3</code></a> Fix race condition with X509Name creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a7528056c5be6f3fbabc52c2fd02882b208d5939"><code>a752805</code></a> Document the horror show</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/78aa9aa22cfd58ac33d1e19184cec667438fd2a1"><code>78aa9aa</code></a> Always provide an X509V3Context in X509Extension::new because OpenSSL require...</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/332311b597cc444a10d4acaf122ee58bd1bc8ff8"><code>332311b</code></a> Resolve an injection vulnerability in EKU creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/482575bff434f58b80ffea34a9610d0ff265ac1f"><code>482575b</code></a> Resolve an injection vulnerability in SAN creation</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/690eeb2ac20d47e43f04d8cb43f03d4128946b81"><code>690eeb2</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1852">#1852</a> from smoelius/master</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/e5b6d97ed170f835b56440d79edcd46381a46ebc"><code>e5b6d97</code></a> Improve reliability of some tests</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/319200ab93e252a3c0e127adc1e4c43a90f063a1"><code>319200a</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/1851">#1851</a> from alex/libressl-versions</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.32...openssl-v0.10.48">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.32&new-version=0.10.48)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-25 00:11:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2342" class=".btn">#2342</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): fix v2-2-x/deploy-lock-asset.test.ts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Telling the typescript compiler to skip the library code check so that
auto-updating dependencies don't break the test fixture chain code
compilation.

The root cause and the fix are equivalent as they were for:
https://github.com/hyperledger/cacti/issues/2322
https://github.com/hyperledger/cacti/pull/2323
Commit SHA: dfb727861b5e26a15dbef0729a2a14dd26b4655f

Fixes #2341

Also sneaking in a .gitignore change with this: there is a VSCode
extension that stores local editing history of files in a .history/
sub-folder and that needs to be ignored in git otherwise it just keeps
popping up in the git index which is annoying sometimes.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 16:42:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2340" class=".btn">#2340</a>
            </td>
            <td>
                <b>
                    chore(tools): script to bump openapi spec dependency versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2206
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 07:20:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2339" class=".btn">#2339</a>
            </td>
            <td>
                <b>
                    build(plugin-keychain-vault): fix CVE-2021-32810 - upgrade vault crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Verified that these changes are okay by recompiling the rust code
and executing the manual steps from the readme that launch the containers
and then uses cURL to send a couple of requests in.

Fixes #2338

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 23:54:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2337" class=".btn">#2337</a>
            </td>
            <td>
                <b>
                    docs(release): add RELEASE_MANAGEMENT.md file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2336

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 03:01:01 +0000 UTC
    </div>
</div>

