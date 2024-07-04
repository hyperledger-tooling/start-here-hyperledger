---
layout: default
title: identus-mediator
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/identus-mediator
---

# identus-mediator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus-mediator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-mediator/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    Update zio, zio-test, zio-test-magnolia, ... to 2.1.5 in main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## About this PR
📦 Updates 
* [dev.zio:zio](https://github.com/zio/zio)
* [dev.zio:zio-test](https://github.com/zio/zio)
* [dev.zio:zio-test-magnolia](https://github.com/zio/zio)
* [dev.zio:zio-test-sbt](https://github.com/zio/zio)

 from `2.0.22` to `2.1.5`

📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.5) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.5)

## Usage
✅ **Please merge!**

I'll automatically update this PR to resolve conflicts as long as you don't change it yourself.

If you'd like to skip this version, you can just close this PR. If you have any feedback, just mention me in the comments below.

Configure Scala Steward for your repository with a [`.scala-steward.conf`](https://github.com/scala-steward-org/scala-steward/blob/767fcfecbfd53c507152f6cf15c846176bae561d/docs/repo-specific-configuration.md) file.

_Have a fantastic day writing Scala!_

<details>
<summary>⚙ Adjust future updates</summary>

Add this to your `.scala-steward.conf` file to ignore future updates of this dependency:
```
updates.ignore = [ { groupId = "dev.zio" } ]
```
Or, add this to slow down future updates of this dependency:
```
dependencyOverrides = [{
  pullRequests = { frequency = "30 days" },
  dependency = { groupId = "dev.zio" }
}]
```
</details>

<sup>
labels: library-update, early-semver-minor, semver-spec-minor, commit-count:1
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 20:02:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-mediator/pull/323" class=".btn">#323</a>
            </td>
            <td>
                <b>
                    Update zio-json to 0.7.1 in main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## About this PR
📦 Updates [dev.zio:zio-json](https://github.com/zio/zio-json) from `0.6.2` to `0.7.1`

📜 [GitHub Release Notes](https://github.com/zio/zio-json/releases/tag/v0.7.1) - [Version Diff](https://github.com/zio/zio-json/compare/v0.6.2...v0.7.1)

## Usage
✅ **Please merge!**

I'll automatically update this PR to resolve conflicts as long as you don't change it yourself.

If you'd like to skip this version, you can just close this PR. If you have any feedback, just mention me in the comments below.

Configure Scala Steward for your repository with a [`.scala-steward.conf`](https://github.com/scala-steward-org/scala-steward/blob/767fcfecbfd53c507152f6cf15c846176bae561d/docs/repo-specific-configuration.md) file.

_Have a fantastic day writing Scala!_

<details>
<summary>🔍 Files still referring to the old version number</summary>

The following files still refer to the old version number (0.6.2).
You might want to review and update them manually.
```
package-lock.json
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add this to your `.scala-steward.conf` file to ignore future updates of this dependency:
```
updates.ignore = [ { groupId = "dev.zio", artifactId = "zio-json" } ]
```
Or, add this to slow down future updates of this dependency:
```
dependencyOverrides = [{
  pullRequests = { frequency = "30 days" },
  dependency = { groupId = "dev.zio", artifactId = "zio-json" }
}]
```
</details>

<sup>
labels: library-update, early-semver-major, semver-spec-minor, old-version-remains, commit-count:1
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-27 20:03:10 +0000 UTC
    </div>
</div>

