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
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1102" class=".btn">#1102</a>
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

* 📦 [com.github.sbt:sbt-native-packager](https://github.com/sbt/sbt-native-packager) from `1.9.16` to `1.10.0`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-native-packager/releases/tag/v1.10.0) - [Changelog](https://github.com/sbt/sbt-native-packager/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/sbt/sbt-native-packager/compare/v1.9.16...v1.10.0)
* 📦 [org.scalameta:munit](https://github.com/scalameta/munit) from `1.0.0-RC1` to `1.0.0`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/munit/releases/tag/v1.0.0) - [Version Diff](https://github.com/scalameta/munit/compare/v1.0.0-RC1...v1.0.0)

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
  { groupId = "com.github.sbt", artifactId = "sbt-native-packager" },
  { groupId = "org.scalameta", artifactId = "munit" }
]
```
Or, add these to slow down future updates of these dependencies:
```
dependencyOverrides = [
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.github.sbt", artifactId = "sbt-native-packager" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scalameta", artifactId = "munit" }
  }
]
```
</details>

<sup>
labels: sbt-plugin-update, test-library-update, early-semver-minor, semver-spec-minor, early-semver-pre-release, semver-spec-pre-release, old-version-remains, commit-count:n:2
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-26 00:19:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1101" class=".btn">#1101</a>
            </td>
            <td>
                <b>
                    build: DAL dependency update
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

* 📦 [io.getquill:quill-doobie](https://github.com/zio/zio-protoquill) from `4.8.4` to `4.8.5`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-protoquill/releases/tag/v4.8.5) - [Changelog](https://github.com/zio/zio-protoquill/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/zio/zio-protoquill/compare/v4.8.4...v4.8.5)
* 📦 [io.getquill:quill-jdbc-zio](https://github.com/zio/zio-protoquill) from `4.8.4` to `4.8.5`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-protoquill/releases/tag/v4.8.5) - [Changelog](https://github.com/zio/zio-protoquill/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/zio/zio-protoquill/compare/v4.8.4...v4.8.5)

## Usage
✅ **Please merge!**

I'll automatically update this PR to resolve conflicts as long as you don't change it yourself.

If you have any feedback, just mention me in the comments below.

Configure Scala Steward for your repository with a [`.scala-steward.conf`](https://github.com/scala-steward-org/scala-steward/blob/767fcfecbfd53c507152f6cf15c846176bae561d/docs/repo-specific-configuration.md) file.

_Have a fantastic day writing Scala!_

<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "io.getquill", artifactId = "quill-doobie" },
  { groupId = "io.getquill", artifactId = "quill-jdbc-zio" }
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
  }
]
```
</details>

<sup>
labels: library-update, early-semver-patch, semver-spec-patch, version-scheme:always, commit-count:1
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-26 00:19:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1100" class=".btn">#1100</a>
            </td>
            <td>
                <b>
                    build: zio dependency updates
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

* 📦 [dev.zio:zio](https://github.com/zio/zio) from `2.0.22` to `2.1.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.1) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.1)
* 📦 [dev.zio:zio-concurrent](https://github.com/zio/zio) from `2.0.22` to `2.1.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.1) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.1)
* 📦 [dev.zio:zio-config](https://github.com/zio/zio-config) from `4.0.1` to `4.0.2`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-config/releases/tag/v4.0.2) - [Version Diff](https://github.com/zio/zio-config/compare/v4.0.1...v4.0.2)
* 📦 [dev.zio:zio-config-magnolia](https://github.com/zio/zio-config) from `4.0.1` to `4.0.2`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-config/releases/tag/v4.0.2) - [Version Diff](https://github.com/zio/zio-config/compare/v4.0.1...v4.0.2)
* 📦 [dev.zio:zio-config-typesafe](https://github.com/zio/zio-config) from `4.0.1` to `4.0.2`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-config/releases/tag/v4.0.2) - [Version Diff](https://github.com/zio/zio-config/compare/v4.0.1...v4.0.2)
* 📦 [dev.zio:zio-http](https://github.com/zio/zio-http) from `3.0.0-RC6` to `3.0.0-RC7`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-http/releases/tag/v3.0.0-RC7) - [Version Diff](https://github.com/zio/zio-http/compare/v3.0.0-RC6...v3.0.0-RC7)
* 📦 [dev.zio:zio-logging](https://github.com/zio/zio-logging) from `2.1.17` to `2.2.4`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-logging/releases/tag/v2.2.4) - [Version Diff](https://github.com/zio/zio-logging/compare/v2.1.17...v2.2.4)
* 📦 [dev.zio:zio-logging-slf4j](https://github.com/zio/zio-logging) from `2.1.17` to `2.2.4`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-logging/releases/tag/v2.2.4) - [Version Diff](https://github.com/zio/zio-logging/compare/v2.1.17...v2.2.4)
* 📦 [dev.zio:zio-prelude](https://github.com/zio/zio-prelude) from `1.0.0-RC24` to `1.0.0-RC26`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-prelude/releases/tag/v1.0.0-RC26) - [Version Diff](https://github.com/zio/zio-prelude/compare/v1.0.0-RC24...v1.0.0-RC26)
* 📦 [dev.zio:zio-test](https://github.com/zio/zio) from `2.0.22` to `2.1.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.1) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.1)
* 📦 [dev.zio:zio-test-magnolia](https://github.com/zio/zio) from `2.0.22` to `2.1.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.1) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.1)
* 📦 [dev.zio:zio-test-sbt](https://github.com/zio/zio) from `2.0.22` to `2.1.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.1) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.1)

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
package-lock.json
tests/performance-tests/agent-performance-tests-k6/yarn.lock
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "dev.zio", artifactId = "zio" },
  { groupId = "dev.zio", artifactId = "zio-concurrent" },
  { groupId = "dev.zio", artifactId = "zio-config" },
  { groupId = "dev.zio", artifactId = "zio-config-magnolia" },
  { groupId = "dev.zio", artifactId = "zio-config-typesafe" },
  { groupId = "dev.zio", artifactId = "zio-http" },
  { groupId = "dev.zio", artifactId = "zio-logging" },
  { groupId = "dev.zio", artifactId = "zio-logging-slf4j" },
  { groupId = "dev.zio", artifactId = "zio-prelude" },
  { groupId = "dev.zio", artifactId = "zio-test" },
  { groupId = "dev.zio", artifactId = "zio-test-magnolia" },
  { groupId = "dev.zio", artifactId = "zio-test-sbt" }
]
```
Or, add these to slow down future updates of these dependencies:
```
dependencyOverrides = [
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-concurrent" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-config" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-config-magnolia" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-config-typesafe" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-http" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-logging" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-logging-slf4j" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-prelude" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-test" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-test-magnolia" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-test-sbt" }
  }
]
```
</details>

<sup>
labels: library-update, test-library-update, early-semver-minor, semver-spec-minor, early-semver-patch, semver-spec-patch, early-semver-pre-release, semver-spec-pre-release, old-version-remains, commit-count:n:5
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-26 00:19:02 +0000 UTC
    </div>
</div>

