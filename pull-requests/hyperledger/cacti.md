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
                PR <a href="https://github.com/hyperledger/cacti/pull/2878" class=".btn">#2878</a>
            </td>
            <td>
                <b>
                    build(connector-corda): fix various Unresolved reference kotlin compiler errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Started overriding a specific template (dataClass.mustache) in the
main-server sub-package of the corda connector because of issues that
are further explained here [1] and here [2].
2. Also had to update generator configuration to specifically exclude
spring-doc generation because it seems to be broken within the template
as well: it does not provide updated dependencies for the grandle and
maven manifests and so the `io.swagger.core.v3:swagger-annotations` package
was missing and failing the build in a second way.
3. The example value for the return array of `ListFlowsV1Response` in
the openapi.json spec file of the corda connector was containing dollar
signs ($) which ended up being appended to the kotlin code's annotations
as documentation, but the dollar signs have a special meaning in kotlin
and lead to syntax errors. Updating the examples to not have dollar signs
in the openapi.json specification document resulted in fixing this issue.
4. Also updated the artifact version in the openapi generator configuration
file. This is just a temporary fix, what we really need is scripts bumping
this up as part of the automated release process.

[1] https://github.com/OpenAPITools/openapi-generator/issues/8366#issuecomment-1799795399
[2] https://github.com/OpenAPITools/openapi-generator/pull/17008

Fixes #2662

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
        Created At 2023-11-12 07:58:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2877" class=".btn">#2877</a>
            </td>
            <td>
                <b>
                    feat: cacti polkadot connector
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It's the updated PR for Polkadot support for Cacti that incorporates the efforts of @RafaelAPB  @CatarinaPedreira along with my work during the Hyperledger Mentorship under the mentorship of @jagpreetsinghsasan 

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
        Created At 2023-11-11 21:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2876" class=".btn">#2876</a>
            </td>
            <td>
                <b>
                    build(deps): bump axios from 1.5.1 to 1.6.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [axios](https://github.com/axios/axios) from 1.5.1 to 1.6.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/releases">axios's releases</a>.</em></p>
<blockquote>
<h2>Release v1.6.0</h2>
<h2>Release notes:</h2>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/axios/axios/blob/v1.x/CHANGELOG.md">axios's changelog</a>.</em></p>
<blockquote>
<h1><a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">1.6.0</a> (2023-10-26)</h1>
<h3>Bug Fixes</h3>
<ul>
<li><strong>CSRF:</strong> fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>) (<a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0">96ee232</a>)</li>
<li><strong>dns:</strong> fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>) (<a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8">5aaff53</a>)</li>
<li><strong>types:</strong> fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>) (<a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09">a1c8ad0</a>)</li>
</ul>
<h3>PRs</h3>
<ul>
<li>CVE 2023 45857 ( <a href="https://api.github.com/repos/axios/axios/pulls/6028">#6028</a> )</li>
</ul>
<pre><code>
⚠️ Critical vulnerability fix. See https://security.snyk.io/vuln/SNYK-JS-AXIOS-6032459
</code></pre>
<h3>Contributors to this release</h3>
<ul>
<li><!-- raw HTML omitted --> <a href="https://github.com/DigitalBrainJS" title="+449/-114 ([#6032](https://github.com/axios/axios/issues/6032) [#6021](https://github.com/axios/axios/issues/6021) [#6011](https://github.com/axios/axios/issues/6011) [#5932](https://github.com/axios/axios/issues/5932) [#5931](https://github.com/axios/axios/issues/5931) )">Dmitriy Mozgovoy</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/valentin-panov" title="+4/-4 ([#6028](https://github.com/axios/axios/issues/6028) )">Valentin Panov</a></li>
<li><!-- raw HTML omitted --> <a href="https://github.com/therealrinku" title="+1/-1 ([#5889](https://github.com/axios/axios/issues/5889) )">Rinku Chaudhari</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/axios/axios/commit/f7adacdbaa569281253c8cfc623ad3f4dc909c60"><code>f7adacd</code></a> chore(release): v1.6.0 (<a href="https://redirect.github.com/axios/axios/issues/6031">#6031</a>)</li>
<li><a href="https://github.com/axios/axios/commit/9917e67cbb6c157382863bad8c741de58e3f3c2b"><code>9917e67</code></a> chore(ci): fix release-it arg; (<a href="https://redirect.github.com/axios/axios/issues/6032">#6032</a>)</li>
<li><a href="https://github.com/axios/axios/commit/96ee232bd3ee4de2e657333d4d2191cd389e14d0"><code>96ee232</code></a> fix(CSRF): fixed CSRF vulnerability CVE-2023-45857 (<a href="https://redirect.github.com/axios/axios/issues/6028">#6028</a>)</li>
<li><a href="https://github.com/axios/axios/commit/7d45ab2e2ad6e59f5475e39afd4b286b1f393fc0"><code>7d45ab2</code></a> chore(tests): fixed tests to pass in node v19 and v20 with <code>keep-alive</code> enabl...</li>
<li><a href="https://github.com/axios/axios/commit/5aaff532a6b820bb9ab6a8cd0f77131b47e2adb8"><code>5aaff53</code></a> fix(dns): fixed lookup function decorator to work properly in node v20; (<a href="https://redirect.github.com/axios/axios/issues/6011">#6011</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a48a63ad823fc20e5a6a705f05f09842ca49f48c"><code>a48a63a</code></a> chore(docs): added AxiosHeaders docs; (<a href="https://redirect.github.com/axios/axios/issues/5932">#5932</a>)</li>
<li><a href="https://github.com/axios/axios/commit/a1c8ad008b3c13d53e135bbd0862587fb9d3fc09"><code>a1c8ad0</code></a> fix(types): fix AxiosHeaders types; (<a href="https://redirect.github.com/axios/axios/issues/5931">#5931</a>)</li>
<li><a href="https://github.com/axios/axios/commit/2ac731d60545ba5c4202c25fd2e732ddd8297d82"><code>2ac731d</code></a> chore(docs): update readme.md (<a href="https://redirect.github.com/axios/axios/issues/5889">#5889</a>)</li>
<li>See full diff in <a href="https://github.com/axios/axios/compare/v1.5.1...v1.6.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=axios&package-manager=npm_and_yarn&previous-version=1.5.1&new-version=1.6.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-11-11 16:18:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2875" class=".btn">#2875</a>
            </td>
            <td>
                <b>
                    docs(examples): fix cbdc-bridging-frontend/package.json version 2.0.0-alpha.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Updated the version accordingly.
2. This pull request must be merged before we issue the 2.0.0 release
otherwise the npm package version will be broken on the public registry.

[skip ci]

Fixes #2874

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
        Created At 2023-11-10 19:47:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2873" class=".btn">#2873</a>
            </td>
            <td>
                <b>
                    refactor: project-wide change of OAS vendor extensions cactus -> cacti
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Did a complete find & replace of the old vendor extensions and the
new ones. In theory this is a change that the compiler guarantees for us
to verify completely, but even with that said, I'll leave the CI on so
that we can double check to be sure.
This is also a BREAKING CHANGE because if someone had installed the older
packages and they imported endpoint definitions from the OAS spec based
on the vendor extensions then their could would stop compiling. Therefore
this change must be done before we issue the 2.0.0 release.
2. Also added a bug-fix to tools/custom-checks/check-open-api-json-specs.ts
because it wasn't just validating HTTP verbs within "paths" but also
any property that was in there such as "summary" or "description" but
of course those are string properties so they won't pass the validation
we impose on HTTP verb definitions for the endpoints.

Fixes #2872

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
        Created At 2023-11-10 19:35:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2871" class=".btn">#2871</a>
            </td>
            <td>
                <b>
                    build(tools): fix custom-checks/check-open-api-json-specs error messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. There was no "ERROR:" prefix for some of the problems that the check
was returning making it hard/not so obvious to figure out what the
actual problems are that are making the checks fail overall.

[skip ci]

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
        Created At 2023-11-10 18:43:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2870" class=".btn">#2870</a>
            </td>
            <td>
                <b>
                    ci: add container scanning to default checks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Trivy** is a cutting-edge security tool designed to enhance the safety of containerized applications by conducting thorough vulnerability assessments. Specifically developed for scanning container images, ranging from low-severity issues to critical threats. It employs an intelligent rating system to categorize vulnerabilities based on their severity levels, ensuring that high to critical vulnerabilities are given special attention. Upon detecting vulnerabilities that fall within this elevated range, Trivy will throw an error.

By integrating Trivy into our deployment pipeline, we can proactively mitigate security risks and enhance the resilience of our repository.

Fixes hyperledger#1876

Depends On: hyperledger#2865
Depends On: hyperledger#2864
Depends On: hyperledger#2863
Depends On: hyperledger#2862

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
        Created At 2023-11-10 06:27:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2869" class=".btn">#2869</a>
            </td>
            <td>
                <b>
                    fix(connector-besu): error handling of DeployContractSolidityBytecodeEndpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                1. Uses the new utility function from the core package in the catch block
so that HTTP statusCode is matching the intent of the thrower (e.g.
correctly differentiates between user-error and developer error)
2. Updates the deployContract method of the besu connector so that it
correctly specifies the intent of the errors thrown as either user error
or developer error via setting the statusCode property of the HTTP errors
to either 4xx or 5xx depending on the cause.
3. Provides a template for future similar changes (of which we'll need
dozens to update all the REST API endpoints)

Depends on #2868

Related to but does not conclude: https://github.com/hyperledger/cacti/issues/1747

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 21:33:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2868" class=".btn">#2868</a>
            </td>
            <td>
                <b>
                    feat(cactus-core): add handleRestEndpointException utility to public API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This is a function that is designed to be called by all the REST API
endpoint implementations to (more) correctly handle errors.
2. The problem right now is that we do not differentiate between invalid
request errors (e.g. expected exceptions) vs.
legitimate crashes (e.g. unexpected exceptions)
What the above means is that a lot of our endpoints will crash with an
HTTP 500 error code returned to the client even if the problem as user-
error (such as a missing parameter that is mandatory).
3. With the new utility function the REST endpoint code can easily
apply the decision logic at runtime in their own catch blocks' and
set the HTTP response status code based on the information (context)
provided by the callee (most often the connector plugin's underlying
method that was called)

An example usage of this utility method can be described as:
1. Add the necessary dependencies to your plugin (`http-errors`, `@types/http-errors`)
2. `yarn install` (which will update the lock file)
3. Choose the endpoint you wish to update to be using the new handleRestEndpointException
function internally when handling HTTP requests that involve the plugin.
For example this file:
```
packages/cactus-plugin-ledger-connector-besu/src/main/typescript/
web-services/deploy-contract-solidity-bytecode-endpoint.ts
```
4. Update the `catch() { ... }` block of the `handleRequest` method to
invoke the handleRestEndpointException method:

```typescript
public async handleRequest(req: Request, res: Response): Promise<void> {
const fnTag = `${this.className}#handleRequest()`;
const reqTag = `${this.getVerbLowerCase()} - ${this.getPath()}`;
this.log.debug(reqTag);
const reqBody: DeployContractSolidityBytecodeV1Request = req.body;
try {
    const resBody = await this.options.connector.deployContract(reqBody);
    res.json(resBody);
} catch (ex) {
    const errorMsg = `${reqTag} ${fnTag} Failed to deploy contract:`;
    handleRestEndpointException({ errorMsg, log: this.log, error: ex, res });
}
}
```

Then proceed to also update the implementation of the method that is  being
called by the REST endpoint request handler such that it uses the HTTP
errors according to their intended status codes, e.g. 400 is user error
and 5xx is something that is a developer error (e.g. indicating that
a bug is in the code of the plugin and should be fixed)

```typescript
import createHttpError from "http-errors";

export class SomePluginImplementration {

  public async deployContract(
    req: DeployContractSolidityBytecodeV1Request,
  ): Promise<DeployContractSolidityBytecodeV1Response> {
    const fnTag = `${this.className}#deployContract()`;
    Checks.truthy(req, `${fnTag} req`);
    if (isWeb3SigningCredentialNone(req.web3SigningCredential)) {
      throw createHttpError[400](
        `${fnTag} Cannot deploy contract with pre-signed TX`,
      );
    }
    const { keychainId, contractName } = req;
    if (!keychainId || !req.contractName) {
      const errorMessage = `${fnTag} Cannot deploy contract without keychainId and the contractName.`;
      throw createHttpError[400](errorMessage);
    }

    const keychainPlugin = this.pluginRegistry.findOneByKeychainId(keychainId);

    if (!keychainPlugin) {
      const errorMessage =
        `${fnTag} The plugin registry does not contain` +
        ` a keychain plugin for ID:"${req.keychainId}"`;
      throw createHttpError[400](errorMessage);
    }

    if (!keychainPlugin.has(contractName)) {
      const errorMessage =
        `${fnTag} Cannot create an instance of the contract instance because` +
        `the contractName in the request does not exist on the keychain`;
      throw new createHttpError[400](errorMessage);
    }
    // rest of the implementation goes here
}
```

[skip ci]

Related to, but does NOT conclude: https://github.com/hyperledger/cacti/issues/1747

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
        Created At 2023-11-09 21:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2867" class=".btn">#2867</a>
            </td>
            <td>
                <b>
                    build(dev-container): add git auto-completion via .bashrc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2215

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
        Created At 2023-11-09 20:05:50 +0000 UTC
    </div>
</div>

