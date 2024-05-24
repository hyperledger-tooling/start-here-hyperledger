---
layout: default
title: identus-cloud-agent
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/identus-cloud-agent
---

# identus-cloud-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus-cloud-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1078" class=".btn">#1078</a>
            </td>
            <td>
                <b>
                    build: sbt and plugins dependency update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span>
            </td>
            <td>
                ## About this PR
Updates:

* 📦 [com.eed3si9n:sbt-buildinfo](https://github.com/sbt/sbt-buildinfo) from `0.11.0` to `0.12.0`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-buildinfo/releases/tag/v0.12.0) - [Version Diff](https://github.com/sbt/sbt-buildinfo/compare/v0.11.0...v0.12.0)
* 📦 [com.github.sbt:sbt-native-packager](https://github.com/sbt/sbt-native-packager) from `1.9.11` to `1.9.16`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-native-packager/releases/tag/v1.9.16) - [Changelog](https://github.com/sbt/sbt-native-packager/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/sbt/sbt-native-packager/compare/v1.9.11...v1.9.16)
* 📦 [com.github.sbt:sbt-release](https://github.com/sbt/sbt-release) from `1.1.0` to `1.4.0`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-release/releases/tag/v1.4.0) - [Version Diff](https://github.com/sbt/sbt-release/compare/v1.1.0...v1.4.0)
* 📦 [org.scala-sbt:sbt](https://github.com/sbt/sbt) from `1.9.9` to `1.10.0`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt/releases/tag/v1.10.0) - [Version Diff](https://github.com/sbt/sbt/compare/v1.9.9...v1.10.0)
* 📦 [org.scalameta:sbt-scalafmt](https://github.com/scalameta/sbt-scalafmt) from `2.5.0` to `2.5.2`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/sbt-scalafmt/releases/tag/v2.5.2) - [Version Diff](https://github.com/scalameta/sbt-scalafmt/compare/v2.5.0...v2.5.2)
* 📦 [org.scalameta:scalafmt-core](https://github.com/scalameta/scalafmt) from `3.7.17` to `3.8.1`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/scalafmt/releases/tag/v3.8.1) - [Version Diff](https://github.com/scalameta/scalafmt/compare/v3.7.17...v3.8.1)
* 📦 [org.scoverage:sbt-coveralls](https://github.com/scoverage/sbt-coveralls) from `1.3.9` to `1.3.11`
  + 📜 [GitHub Release Notes](https://github.com/scoverage/sbt-coveralls/releases/tag/v1.3.11) - [Version Diff](https://github.com/scoverage/sbt-coveralls/compare/v1.3.9...v1.3.11)
* 📦 [org.scoverage:sbt-scoverage](https://github.com/scoverage/sbt-scoverage) from `2.0.6` to `2.0.12`
  + 📜 [GitHub Release Notes](https://github.com/scoverage/sbt-scoverage/releases/tag/v2.0.12) - [Version Diff](https://github.com/scoverage/sbt-scoverage/compare/v2.0.6...v2.0.12)

## Usage
✅ **Please merge!**

I'll automatically update this PR to resolve conflicts as long as you don't change it yourself.

If you have any feedback, just mention me in the comments below.

Configure Scala Steward for your repository with a [`.scala-steward.conf`](https://github.com/scala-steward-org/scala-steward/blob/767fcfecbfd53c507152f6cf15c846176bae561d/docs/repo-specific-configuration.md) file.

_Have a fantastic day writing Scala!_

<details>
<summary>🔍 Files still referring to the old version numbers</summary>

The following files still refer to the old version numbers.
You might want to review and update them manually.
```
CHANGELOG.md
DEPENDENCIES.md
cloud-agent/service/CHANGELOG.md
connect/CHANGELOG.md
mercury/CHANGELOG.md
package-lock.json
pollux/CHANGELOG.md
cloud-agent/client/generator/yarn.lock
cloud-agent/service/api/http/cloud-agent-openapi-spec.yaml
cloud-agent/service/server/src/main/scala/org/hyperledger/identus/system/controller/http/HealthInfo.scala
docs/docusaurus/schemas/update.md
tests/performance-tests/agent-performance-tests-k6/yarn.lock
.git-blame-ignore-revs
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "com.eed3si9n", artifactId = "sbt-buildinfo" },
  { groupId = "com.github.sbt", artifactId = "sbt-native-packager" },
  { groupId = "com.github.sbt", artifactId = "sbt-release" },
  { groupId = "org.scala-sbt", artifactId = "sbt" },
  { groupId = "org.scalameta", artifactId = "sbt-scalafmt" },
  { groupId = "org.scalameta", artifactId = "scalafmt-core" },
  { groupId = "org.scoverage", artifactId = "sbt-coveralls" },
  { groupId = "org.scoverage", artifactId = "sbt-scoverage" }
]
```
Or, add these to slow down future updates of these dependencies:
```
dependencyOverrides = [
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.eed3si9n", artifactId = "sbt-buildinfo" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.github.sbt", artifactId = "sbt-native-packager" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.github.sbt", artifactId = "sbt-release" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scala-sbt", artifactId = "sbt" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scalameta", artifactId = "sbt-scalafmt" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scalameta", artifactId = "scalafmt-core" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scoverage", artifactId = "sbt-coveralls" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scoverage", artifactId = "sbt-scoverage" }
  }
]
```
</details>

<sup>
labels: sbt-plugin-update, library-update, early-semver-major, semver-spec-minor, early-semver-patch, semver-spec-patch, early-semver-minor, version-scheme:early-semver, old-version-remains, commit-count:n:8
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 11:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1077" class=".btn">#1077</a>
            </td>
            <td>
                <b>
                    build: protobuf dependency update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">build</span>
            </td>
            <td>
                ## About this PR
Updates:

* 📦 [com.thesamet.scalapb:compilerplugin](https://github.com/scalapb/ScalaPB) from `0.11.13` to `0.11.15`
  + 📜 [GitHub Release Notes](https://github.com/scalapb/ScalaPB/releases/tag/v0.11.15) - [Changelog](https://github.com/scalapb/ScalaPB/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/scalapb/ScalaPB/compare/v0.11.13...v0.11.15)
* 📦 [com.thesamet.scalapb:scalapb-runtime-grpc](https://github.com/scalapb/ScalaPB) from `0.11.13` to `0.11.15`
  + 📜 [GitHub Release Notes](https://github.com/scalapb/ScalaPB/releases/tag/v0.11.15) - [Changelog](https://github.com/scalapb/ScalaPB/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/scalapb/ScalaPB/compare/v0.11.13...v0.11.15)

## Usage
✅ **Please merge!**

I'll automatically update this PR to resolve conflicts as long as you don't change it yourself.

If you have any feedback, just mention me in the comments below.

Configure Scala Steward for your repository with a [`.scala-steward.conf`](https://github.com/scala-steward-org/scala-steward/blob/767fcfecbfd53c507152f6cf15c846176bae561d/docs/repo-specific-configuration.md) file.

_Have a fantastic day writing Scala!_

<details>
<summary>🔍 Files still referring to the old version numbers</summary>

The following files still refer to the old version numbers.
You might want to review and update them manually.
```
DEPENDENCIES.md
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "com.thesamet.scalapb", artifactId = "compilerplugin" },
  { groupId = "com.thesamet.scalapb", artifactId = "scalapb-runtime-grpc" }
]
```
Or, add these to slow down future updates of these dependencies:
```
dependencyOverrides = [
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.thesamet.scalapb", artifactId = "compilerplugin" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.thesamet.scalapb", artifactId = "scalapb-runtime-grpc" }
  }
]
```
</details>

<sup>
labels: library-update, early-semver-minor, semver-spec-patch, version-scheme:early-semver, old-version-remains, commit-count:1
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 11:21:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1076" class=".btn">#1076</a>
            </td>
            <td>
                <b>
                    build: DAL dependency update
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">build</span><span class="chip">shared</span>
            </td>
            <td>
                ## About this PR
Updates:

* 📦 [io.getquill:quill-doobie](https://github.com/zio/zio-protoquill) from `4.7.3` to `4.8.4`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-protoquill/releases/tag/v4.8.4) - [Changelog](https://github.com/zio/zio-protoquill/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/zio/zio-protoquill/compare/v4.7.3...v4.8.4)
* 📦 [io.getquill:quill-jdbc-zio](https://github.com/zio/zio-protoquill) from `4.7.3` to `4.8.4`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-protoquill/releases/tag/v4.8.4) - [Changelog](https://github.com/zio/zio-protoquill/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/zio/zio-protoquill/compare/v4.7.3...v4.8.4)
* 📦 [org.postgresql:postgresql](https://github.com/pgjdbc/pgjdbc) from `42.2.29` to `42.7.3`
  + 📜 [Changelog](https://github.com/pgjdbc/pgjdbc/blob/master/CHANGELOG.md)
* 📦 [org.tpolecat:doobie-hikari](https://github.com/tpolecat/doobie) from `1.0.0-RC2` to `1.0.0-RC5`
  + 📜 [GitHub Release Notes](https://github.com/tpolecat/doobie/releases/tag/v1.0.0-RC5) - [Version Diff](https://github.com/tpolecat/doobie/compare/v1.0.0-RC2...v1.0.0-RC5)
* 📦 [org.tpolecat:doobie-postgres](https://github.com/tpolecat/doobie) from `1.0.0-RC2` to `1.0.0-RC5`
  + 📜 [GitHub Release Notes](https://github.com/tpolecat/doobie/releases/tag/v1.0.0-RC5) - [Version Diff](https://github.com/tpolecat/doobie/compare/v1.0.0-RC2...v1.0.0-RC5)
* 📦 [org.tpolecat:doobie-postgres-circe](https://github.com/tpolecat/doobie) from `1.0.0-RC2` to `1.0.0-RC5`
  + 📜 [GitHub Release Notes](https://github.com/tpolecat/doobie/releases/tag/v1.0.0-RC5) - [Version Diff](https://github.com/tpolecat/doobie/compare/v1.0.0-RC2...v1.0.0-RC5)

## Usage
✅ **Please merge!**

I'll automatically update this PR to resolve conflicts as long as you don't change it yourself.

If you have any feedback, just mention me in the comments below.

Configure Scala Steward for your repository with a [`.scala-steward.conf`](https://github.com/scala-steward-org/scala-steward/blob/767fcfecbfd53c507152f6cf15c846176bae561d/docs/repo-specific-configuration.md) file.

_Have a fantastic day writing Scala!_

<details>
<summary>🔍 Files still referring to the old version numbers</summary>

The following files still refer to the old version numbers.
You might want to review and update them manually.
```
DEPENDENCIES.md
build.sbt
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "io.getquill", artifactId = "quill-doobie" },
  { groupId = "io.getquill", artifactId = "quill-jdbc-zio" },
  { groupId = "org.postgresql", artifactId = "postgresql" },
  { groupId = "org.tpolecat", artifactId = "doobie-hikari" },
  { groupId = "org.tpolecat", artifactId = "doobie-postgres" },
  { groupId = "org.tpolecat", artifactId = "doobie-postgres-circe" }
]
```
Or, add these to slow down future updates of these dependencies:
```
dependencyOverrides = [
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "io.getquill", artifactId = "quill-doobie" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "io.getquill", artifactId = "quill-jdbc-zio" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.postgresql", artifactId = "postgresql" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.tpolecat", artifactId = "doobie-hikari" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.tpolecat", artifactId = "doobie-postgres" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.tpolecat", artifactId = "doobie-postgres-circe" }
  }
]
```
</details>

<sup>
labels: library-update, early-semver-minor, semver-spec-minor, version-scheme:always, early-semver-pre-release, semver-spec-pre-release, version-scheme:early-semver, old-version-remains, commit-count:n:3
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 11:21:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1074" class=".btn">#1074</a>
            </td>
            <td>
                <b>
                    ci: scala steward DCO by hardcoding the message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
- implemented workaround to configure the DCO for the Scala Steward bot

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 09:55:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1071" class=".btn">#1071</a>
            </td>
            <td>
                <b>
                    test: add DID Registrar test scenario to use new key types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span>
            </td>
            <td>
                ### Description: 
Summarize the changes you're submitting in a few sentences, including Jira ticket ATL-xxxx if applicable.
Link to any discussion, related issues and bug reports to give the context to help the reviewer understand the PR.

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 08:36:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1070" class=".btn">#1070</a>
            </td>
            <td>
                <b>
                    chore(deps): bump requests from 2.26.0 to 2.32.0 in /infrastructure/utils/python/github-helpers in the pip group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update in the /infrastructure/utils/python/github-helpers directory: [requests](https://github.com/psf/requests).

Updates `requests` from 2.26.0 to 2.32.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.0</h2>
<h2>2.32.0 (2024-05-20)</h2>
<h2>🐍 PYCON US 2024 EDITION 🐍</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<p><strong>Deprecations</strong></p>
<ul>
<li>Requests has officially added support for CPython 3.12 (<a href="https://redirect.github.com/psf/requests/issues/6503">#6503</a>)</li>
<li>Requests has officially added support for PyPy 3.9 and 3.10 (<a href="https://redirect.github.com/psf/requests/issues/6641">#6641</a>)</li>
<li>Requests has officially dropped support for CPython 3.7 (<a href="https://redirect.github.com/psf/requests/issues/6642">#6642</a>)</li>
<li>Requests has officially dropped support for PyPy 3.7 and 3.8 (<a href="https://redirect.github.com/psf/requests/issues/6641">#6641</a>)</li>
</ul>
<p><strong>Documentation</strong></p>
<ul>
<li>Various typo fixes and doc improvements.</li>
</ul>
<p><strong>Packaging</strong></p>
<ul>
<li>Requests has started adopting some modern packaging practices.
The source files for the projects (formerly <code>requests</code>) is now located
in <code>src/requests</code> in the Requests sdist. (<a href="https://redirect.github.com/psf/requests/issues/6506">#6506</a>)</li>
<li>Starting in Requests 2.33.0, Requests will migrate to a PEP 517 build system
using <code>hatchling</code>. This should not impact the average user, but extremely old
versions of packaging utilities may have issues with the new packaging format.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/matthewarmand"><code>@​matthewarmand</code></a> made their first contribution in <a href="https://redirect.github.com/psf/requests/pull/6258">psf/requests#6258</a></li>
<li><a href="https://github.com/cpzt"><code>@​cpzt</code></a> made their first contribution in <a href="https://redirect.github.com/psf/requests/pull/6456">psf/requests#6456</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.0 (2024-05-20)</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<p><strong>Deprecations</strong></p>
<ul>
<li>Requests has officially added support for CPython 3.12 (<a href="https://redirect.github.com/psf/requests/issues/6503">#6503</a>)</li>
<li>Requests has officially added support for PyPy 3.9 and 3.10 (<a href="https://redirect.github.com/psf/requests/issues/6641">#6641</a>)</li>
<li>Requests has officially dropped support for CPython 3.7 (<a href="https://redirect.github.com/psf/requests/issues/6642">#6642</a>)</li>
<li>Requests has officially dropped support for PyPy 3.7 and 3.8 (<a href="https://redirect.github.com/psf/requests/issues/6641">#6641</a>)</li>
</ul>
<p><strong>Documentation</strong></p>
<ul>
<li>Various typo fixes and doc improvements.</li>
</ul>
<p><strong>Packaging</strong></p>
<ul>
<li>Requests has started adopting some modern packaging practices.
The source files for the projects (formerly <code>requests</code>) is now located
in <code>src/requests</code> in the Requests sdist. (<a href="https://redirect.github.com/psf/requests/issues/6506">#6506</a>)</li>
<li>Starting in Requests 2.33.0, Requests will migrate to a PEP 517 build system
using <code>hatchling</code>. This should not impact the average user, but extremely old
versions of packaging utilities may have issues with the new packaging format.</li>
</ul>
<h2>2.31.0 (2023-05-22)</h2>
<p><strong>Security</strong></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/d6ebc4a2f1f68b7e355fb7e4dd5ffc0845547f9f"><code>d6ebc4a</code></a> v2.32.0</li>
<li><a href="https://github.com/psf/requests/commit/9a40d1277807f0a4f26c9a37eea8ec90faa8aadc"><code>9a40d12</code></a> Avoid reloading root certificates to improve concurrent performance (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li><a href="https://github.com/psf/requests/commit/0c030f78d24f29a459dbf39b28b4cc765e2153d7"><code>0c030f7</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a> from nateprewitt/no_char_detection</li>
<li><a href="https://github.com/psf/requests/commit/555b870eb19d497ddb67042645420083ec8efb02"><code>555b870</code></a> Allow character detection dependencies to be optional in post-packaging steps</li>
<li><a href="https://github.com/psf/requests/commit/d6dded3f00afcf56a7e866cb0732799045301eb0"><code>d6dded3</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6700">#6700</a> from franekmagiera/update-redirect-to-invalid-uri-test</li>
<li><a href="https://github.com/psf/requests/commit/bf24b7d8d17da34be720c19e5978b2d3bf94a53b"><code>bf24b7d</code></a> Use an invalid URI that will not cause httpbin to throw 500</li>
<li><a href="https://github.com/psf/requests/commit/2d5f54779ad174035c5437b3b3c1146b0eaf60fe"><code>2d5f547</code></a> Pin 3.8 and 3.9 runners back to macos-13 (<a href="https://redirect.github.com/psf/requests/issues/6688">#6688</a>)</li>
<li><a href="https://github.com/psf/requests/commit/f1bb07d39b74d6444e333879f8b8a3d9dd4d2311"><code>f1bb07d</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6687">#6687</a> from psf/dependabot/github_actions/github/codeql-act...</li>
<li><a href="https://github.com/psf/requests/commit/60047ade64b0b882cbc94e047198818ab580911e"><code>60047ad</code></a> Bump github/codeql-action from 3.24.0 to 3.25.0</li>
<li><a href="https://github.com/psf/requests/commit/31ebb8102c00f8cf8b396a6356743cca4362e07b"><code>31ebb81</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6682">#6682</a> from frenzymadness/pytest8</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.26.0...v2.32.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.26.0&new-version=2.32.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/identus-cloud-agent/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 01:22:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1066" class=".btn">#1066</a>
            </td>
            <td>
                <b>
                    fix: expose new key types in rest api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">castor</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
Expose ability to select key types when creating / updating managed DID. This will soon be released in order to publish the TS and Kotlin client for integration testing. Also add minor alignment on the DID operation validation with Node.
For ATL-7135

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 10:14:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1063" class=".btn">#1063</a>
            </td>
            <td>
                <b>
                    fix: rename the folder to identus for vc-jwt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span>
            </td>
            <td>
                ### Description: 
missing renaming of the folder for vc-jwt

### Alternatives Considered (optional): 
Link to existing ADR (Architecture Decision Record), if any. If relevant, describe other approaches explored and the selected approach. Documenting why the methods were not selected will create a knowledge base for future reference, helping prevent others from revisiting less optimal ideas.

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 08:44:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1057" class=".btn">#1057</a>
            </td>
            <td>
                <b>
                    ci: fix scala steward DCO signature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span><span class="chip">docs</span>
            </td>
            <td>
                ### Description: 
- Fix Scala Steward DCO commit signature

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 08:35:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1056" class=".btn">#1056</a>
            </td>
            <td>
                <b>
                    style: apply linters automatic fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 08:33:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1054" class=".btn">#1054</a>
            </td>
            <td>
                <b>
                    style: apply linters automatic fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 08:28:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1053" class=".btn">#1053</a>
            </td>
            <td>
                <b>
                    docs: rename ADRs in the scope of rebranding to the Identus ATL-7050
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                ### Description: 
- rebrand to Identus in the ADRs ATL-7050 and ATL-7078
- delete outdated files

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-20 08:19:12 +0000 UTC
    </div>
</div>

