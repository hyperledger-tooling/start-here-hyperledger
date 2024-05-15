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
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1045" class=".btn">#1045</a>
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
        Created At 2024-05-14 13:42:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1044" class=".btn">#1044</a>
            </td>
            <td>
                <b>
                    test: add tests for the new key types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">shared</span><span class="chip">mercury</span><span class="chip">castor</span><span class="chip">cloud-agent</span>
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
        Created At 2024-05-14 11:44:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1043" class=".btn">#1043</a>
            </td>
            <td>
                <b>
                    refactor: remove usage of secp256r1 and demos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">build</span>
            </td>
            <td>
                ### Description: 
Remove usage of `secp256r1` in test sources and files used for demo of jwt creds in the past

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
        Created At 2024-05-14 00:06:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1041" class=".btn">#1041</a>
            </td>
            <td>
                <b>
                    perf: update ts client in the performance tests, cleanup `println`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mercury</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
- in the scope of ATL-6404
- cleanup `println` from the production code
- update dependency in the performance test

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 13:49:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1040" class=".btn">#1040</a>
            </td>
            <td>
                <b>
                    build: scala-steward dependency updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## About this PR
Updates:

* 📦 [ch.qos.logback:logback-classic](https://github.com/qos-ch/logback) from `1.4.14` to `1.5.6`
* 📦 [com.eed3si9n:sbt-buildinfo](https://github.com/sbt/sbt-buildinfo) from `0.11.0` to `0.12.0`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-buildinfo/releases/tag/v0.12.0) - [Version Diff](https://github.com/sbt/sbt-buildinfo/compare/v0.11.0...v0.12.0)
* 📦 [com.github.jwt-scala:jwt-circe](https://github.com/jwt-scala/jwt-scala) from `9.4.6` to `10.0.1` ⚠
  + 📜 [GitHub Release Notes](https://github.com/jwt-scala/jwt-scala/releases/tag/v10.0.1) - [Version Diff](https://github.com/jwt-scala/jwt-scala/compare/v9.4.6...v10.0.1)
* 📦 [com.github.sbt:sbt-native-packager](https://github.com/sbt/sbt-native-packager) from `1.9.11` to `1.9.16`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-native-packager/releases/tag/v1.9.16) - [Changelog](https://github.com/sbt/sbt-native-packager/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/sbt/sbt-native-packager/compare/v1.9.11...v1.9.16)
* 📦 [com.github.sbt:sbt-release](https://github.com/sbt/sbt-release) from `1.1.0` to `1.4.0`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-release/releases/tag/v1.4.0) - [Version Diff](https://github.com/sbt/sbt-release/compare/v1.1.0...v1.4.0)
* 📦 [com.networknt:json-schema-validator](https://github.com/networknt/json-schema-validator) from `1.3.2` to `1.3.3`
  + 📜 [GitHub Release Notes](https://github.com/networknt/json-schema-validator/releases/tag/1.3.3) - [Changelog](https://github.com/networknt/json-schema-validator/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/networknt/json-schema-validator/compare/1.3.2...1.3.3)
* 📦 [com.softwaremill.sttp.client3:zio-json](https://github.com/softwaremill/sttp) from `3.8.16` to `3.9.6`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/sttp/releases/tag/v3.9.6) - [Version Diff](https://github.com/softwaremill/sttp/compare/v3.8.16...v3.9.6)
* 📦 [com.softwaremill.sttp.tapir:tapir-http4s-server-zio](https://github.com/softwaremill/tapir) from `1.6.4` to `1.10.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.10.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.10.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-json-zio](https://github.com/softwaremill/tapir) from `1.6.4` to `1.10.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.10.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.10.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-prometheus-metrics](https://github.com/softwaremill/tapir) from `1.6.4` to `1.10.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.10.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.10.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-redoc-bundle](https://github.com/softwaremill/tapir) from `1.6.4` to `1.10.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.10.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.10.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-sttp-stub-server](https://github.com/softwaremill/tapir) from `1.6.4` to `1.10.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.10.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.10.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-swagger-ui-bundle](https://github.com/softwaremill/tapir) from `1.6.4` to `1.10.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.10.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.10.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-zio-http-server](https://github.com/softwaremill/tapir) from `1.6.4` to `1.10.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.10.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.10.7)
* 📦 [com.thesamet:sbt-protoc](https://github.com/thesamet/sbt-protoc) from `1.0.6` to `1.0.7`
  + 📜 [GitHub Release Notes](https://github.com/thesamet/sbt-protoc/releases/tag/v1.0.7) - [Changelog](https://github.com/thesamet/sbt-protoc/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/thesamet/sbt-protoc/compare/v1.0.6...v1.0.7)
* 📦 [com.thesamet.scalapb:compilerplugin](https://github.com/scalapb/ScalaPB) from `0.11.13` to `0.11.15`
  + 📜 [GitHub Release Notes](https://github.com/scalapb/ScalaPB/releases/tag/v0.11.15) - [Changelog](https://github.com/scalapb/ScalaPB/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/scalapb/ScalaPB/compare/v0.11.13...v0.11.15)
* 📦 [com.thesamet.scalapb:scalapb-runtime-grpc](https://github.com/scalapb/ScalaPB) from `0.11.13` to `0.11.15`
  + 📜 [GitHub Release Notes](https://github.com/scalapb/ScalaPB/releases/tag/v0.11.15) - [Changelog](https://github.com/scalapb/ScalaPB/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/scalapb/ScalaPB/compare/v0.11.13...v0.11.15)
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
* 📦 [dev.zio:zio-logging](https://github.com/zio/zio-logging) from `2.1.17` to `2.2.3`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-logging/releases/tag/v2.2.3) - [Version Diff](https://github.com/zio/zio-logging/compare/v2.1.17...v2.2.3)
* 📦 [dev.zio:zio-logging-slf4j](https://github.com/zio/zio-logging) from `2.1.17` to `2.2.3`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-logging/releases/tag/v2.2.3) - [Version Diff](https://github.com/zio/zio-logging/compare/v2.1.17...v2.2.3)
* 📦 [dev.zio:zio-prelude](https://github.com/zio/zio-prelude) from `1.0.0-RC24` to `1.0.0-RC26`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-prelude/releases/tag/v1.0.0-RC26) - [Version Diff](https://github.com/zio/zio-prelude/compare/v1.0.0-RC24...v1.0.0-RC26)
* 📦 [dev.zio:zio-test](https://github.com/zio/zio) from `2.0.22` to `2.1.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.1) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.1)
* 📦 [dev.zio:zio-test-magnolia](https://github.com/zio/zio) from `2.0.22` to `2.1.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.1) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.1)
* 📦 [dev.zio:zio-test-sbt](https://github.com/zio/zio) from `2.0.22` to `2.1.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.1.1) - [Version Diff](https://github.com/zio/zio/compare/v2.0.22...v2.1.1)
* 📦 [io.getquill:quill-doobie](https://github.com/zio/zio-protoquill) from `4.7.3` to `4.8.4`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-protoquill/releases/tag/v4.8.4) - [Changelog](https://github.com/zio/zio-protoquill/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/zio/zio-protoquill/compare/v4.7.3...v4.8.4)
* 📦 [io.getquill:quill-jdbc-zio](https://github.com/zio/zio-protoquill) from `4.7.3` to `4.8.4`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-protoquill/releases/tag/v4.8.4) - [Changelog](https://github.com/zio/zio-protoquill/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/zio/zio-protoquill/compare/v4.7.3...v4.8.4)
* 📦 [io.iohk.atala.prism.apollo:apollo-jvm](https://github.com/input-output-hk/atala-prism-apollo) from `1.2.14` to `1.2.16`
  + 📜 [GitHub Release Notes](https://github.com/input-output-hk/atala-prism-apollo/releases/tag/v1.2.16) - [Version Diff](https://github.com/input-output-hk/atala-prism-apollo/compare/v1.2.14...v1.2.16)
* 📦 [io.micrometer:micrometer-core](https://github.com/micrometer-metrics/micrometer) from `1.11.11` to `1.11.12`
  + 📜 [GitHub Release Notes](https://github.com/micrometer-metrics/micrometer/releases/tag/v1.11.12) - [Version Diff](https://github.com/micrometer-metrics/micrometer/compare/v1.11.11...v1.11.12)
* 📦 [io.micrometer:micrometer-registry-prometheus](https://github.com/micrometer-metrics/micrometer) from `1.11.11` to `1.11.12`
  + 📜 [GitHub Release Notes](https://github.com/micrometer-metrics/micrometer/releases/tag/v1.11.12) - [Version Diff](https://github.com/micrometer-metrics/micrometer/compare/v1.11.11...v1.11.12)
* 📦 [org.flywaydb:flyway-core](https://github.com/flyway/flyway) from `9.22.3` to `10.12.0` ⚠
* 📦 [org.http4s:http4s-blaze-server](https://github.com/http4s/blaze) from `0.23.15` to `0.23.16`
  + 📜 [GitHub Release Notes](https://github.com/http4s/blaze/releases/tag/v0.23.16) - [Version Diff](https://github.com/http4s/blaze/compare/v0.23.15...v0.23.16)
* 📦 [org.postgresql:postgresql](https://github.com/pgjdbc/pgjdbc) from `42.2.29` to `42.7.3`
  + 📜 [Changelog](https://github.com/pgjdbc/pgjdbc/blob/master/CHANGELOG.md)
* 📦 [org.scala-sbt:sbt](https://github.com/sbt/sbt) from `1.9.9` to `1.10.0`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt/releases/tag/v1.10.0) - [Version Diff](https://github.com/sbt/sbt/compare/v1.9.9...v1.10.0)
* 📦 [org.scalameta:sbt-scalafmt](https://github.com/scalameta/sbt-scalafmt) from `2.5.0` to `2.5.2`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/sbt-scalafmt/releases/tag/v2.5.2) - [Version Diff](https://github.com/scalameta/sbt-scalafmt/compare/v2.5.0...v2.5.2)
* 📦 [org.scalameta:scalafmt-core](https://github.com/scalameta/scalafmt) from `3.7.17` to `3.8.1`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/scalafmt/releases/tag/v3.8.1) - [Version Diff](https://github.com/scalameta/scalafmt/compare/v3.7.17...v3.8.1)
* 📦 [org.scalatest:scalatest](https://github.com/scalatest/scalatest) from `3.2.16` to `3.2.18`
  + 📜 [GitHub Release Notes](https://github.com/scalatest/scalatest/releases/tag/release-3.2.18) - [Version Diff](https://github.com/scalatest/scalatest/compare/release-3.2.16...release-3.2.18)
* 📦 [org.scoverage:sbt-coveralls](https://github.com/scoverage/sbt-coveralls) from `1.3.9` to `1.3.11`
  + 📜 [GitHub Release Notes](https://github.com/scoverage/sbt-coveralls/releases/tag/v1.3.11) - [Version Diff](https://github.com/scoverage/sbt-coveralls/compare/v1.3.9...v1.3.11)
* 📦 [org.scoverage:sbt-scoverage](https://github.com/scoverage/sbt-scoverage) from `2.0.6` to `2.0.12`
  + 📜 [GitHub Release Notes](https://github.com/scoverage/sbt-scoverage/releases/tag/v2.0.12) - [Version Diff](https://github.com/scoverage/sbt-scoverage/compare/v2.0.6...v2.0.12)
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
tests/performance-tests/agent-performance-tests-k6/yarn.lock
CHANGELOG.md
cloud-agent/service/CHANGELOG.md
connect/CHANGELOG.md
mercury/CHANGELOG.md
package-lock.json
pollux/CHANGELOG.md
cloud-agent/client/generator/yarn.lock
cloud-agent/service/api/http/cloud-agent-openapi-spec.yaml
cloud-agent/service/server/src/main/scala/org/hyperledger/identus/system/controller/http/HealthInfo.scala
docs/docusaurus/schemas/update.md
build.sbt
.git-blame-ignore-revs
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "ch.qos.logback", artifactId = "logback-classic" },
  { groupId = "com.eed3si9n", artifactId = "sbt-buildinfo" },
  { groupId = "com.github.jwt-scala", artifactId = "jwt-circe" },
  { groupId = "com.github.sbt", artifactId = "sbt-native-packager" },
  { groupId = "com.github.sbt", artifactId = "sbt-release" },
  { groupId = "com.networknt", artifactId = "json-schema-validator" },
  { groupId = "com.softwaremill.sttp.client3", artifactId = "zio-json" },
  { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-http4s-server-zio" },
  { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-json-zio" },
  { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-prometheus-metrics" },
  { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-redoc-bundle" },
  { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-sttp-stub-server" },
  { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-swagger-ui-bundle" },
  { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-zio-http-server" },
  { groupId = "com.thesamet", artifactId = "sbt-protoc" },
  { groupId = "com.thesamet.scalapb", artifactId = "compilerplugin" },
  { groupId = "com.thesamet.scalapb", artifactId = "scalapb-runtime-grpc" },
  { groupId = "dev.zio", artifactId = "zio" },
  { groupId = "dev.zio", artifactId = "zio-concurrent" },
  { groupId = "dev.zio", artifactId = "zio-config" },
  { groupId = "dev.zio", artifactId = "zio-config-magnolia" },
  { groupId = "dev.zio", artifactId = "zio-config-typesafe" },
  { groupId = "dev.zio", artifactId = "zio-logging" },
  { groupId = "dev.zio", artifactId = "zio-logging-slf4j" },
  { groupId = "dev.zio", artifactId = "zio-prelude" },
  { groupId = "dev.zio", artifactId = "zio-test" },
  { groupId = "dev.zio", artifactId = "zio-test-magnolia" },
  { groupId = "dev.zio", artifactId = "zio-test-sbt" },
  { groupId = "io.getquill", artifactId = "quill-doobie" },
  { groupId = "io.getquill", artifactId = "quill-jdbc-zio" },
  { groupId = "io.iohk.atala.prism.apollo", artifactId = "apollo-jvm" },
  { groupId = "io.micrometer", artifactId = "micrometer-core" },
  { groupId = "io.micrometer", artifactId = "micrometer-registry-prometheus" },
  { groupId = "org.flywaydb", artifactId = "flyway-core" },
  { groupId = "org.http4s", artifactId = "http4s-blaze-server" },
  { groupId = "org.postgresql", artifactId = "postgresql" },
  { groupId = "org.scala-sbt", artifactId = "sbt" },
  { groupId = "org.scalameta", artifactId = "sbt-scalafmt" },
  { groupId = "org.scalameta", artifactId = "scalafmt-core" },
  { groupId = "org.scalatest", artifactId = "scalatest" },
  { groupId = "org.scoverage", artifactId = "sbt-coveralls" },
  { groupId = "org.scoverage", artifactId = "sbt-scoverage" },
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
    dependency = { groupId = "ch.qos.logback", artifactId = "logback-classic" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.eed3si9n", artifactId = "sbt-buildinfo" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.github.jwt-scala", artifactId = "jwt-circe" }
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
    dependency = { groupId = "com.networknt", artifactId = "json-schema-validator" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.softwaremill.sttp.client3", artifactId = "zio-json" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-http4s-server-zio" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-json-zio" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-prometheus-metrics" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-redoc-bundle" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-sttp-stub-server" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-swagger-ui-bundle" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.softwaremill.sttp.tapir", artifactId = "tapir-zio-http-server" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.thesamet", artifactId = "sbt-protoc" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.thesamet.scalapb", artifactId = "compilerplugin" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.thesamet.scalapb", artifactId = "scalapb-runtime-grpc" }
  },
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
  },
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
    dependency = { groupId = "io.iohk.atala.prism.apollo", artifactId = "apollo-jvm" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "io.micrometer", artifactId = "micrometer-core" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "io.micrometer", artifactId = "micrometer-registry-prometheus" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.flywaydb", artifactId = "flyway-core" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.http4s", artifactId = "http4s-blaze-server" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.postgresql", artifactId = "postgresql" }
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
    dependency = { groupId = "org.scalatest", artifactId = "scalatest" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scoverage", artifactId = "sbt-coveralls" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.scoverage", artifactId = "sbt-scoverage" }
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
labels: library-update, sbt-plugin-update, test-library-update, early-semver-minor, semver-spec-minor, early-semver-major, semver-spec-major, version-scheme:early-semver, early-semver-patch, semver-spec-patch, early-semver-pre-release, semver-spec-pre-release, version-scheme:always, old-version-remains, commit-count:n:24
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 12:12:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1037" class=".btn">#1037</a>
            </td>
            <td>
                <b>
                    ci: switch Scala Steward to make the PRs as the hyperledger-bot
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span><span class="chip">docs</span>
            </td>
            <td>
                ### Description: 
- change Scala Steward to sign the commits as the Hyperledger Bot
- limit the number of updates in each PR to 10
- add Scala Steward badge to the README.md

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-13 09:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1036" class=".btn">#1036</a>
            </td>
            <td>
                <b>
                    chore: update OID4VCI example script to use issuer metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
Update local script to consume metadata endpoint in the issuance flow. Next, we need to integrate this metadata to `credential` and `credential_offer` endpoint to make this fully functional.

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
        Created At 2024-05-13 09:31:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1032" class=".btn">#1032</a>
            </td>
            <td>
                <b>
                    fix: broken link for the cloud agent packages in readme file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                ### Description: 
After move from IO to Hyperledger organisation and renaming from PRISM agent to Cloud Agent, the Docker packages location was broken. It appears that there are two locations now. So this patch is to update the links in the README file. 

Note that I am not sure if in the end the packages before v1.31.0 will be all moved to the Hyperledger organisation.

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 13:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1031" class=".btn">#1031</a>
            </td>
            <td>
                <b>
                    ci: fix the publishing of ts client [skip ci]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span><span class="chip">cloud-agent</span>
            </td>
            <td>
                ### Description: 
- changed the tag to dispatch the workflow
- use GITHUB_TOKEN to publish ts package to ghcr.io


### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/hyperledger/identus-cloud-agent/blob/main/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [x] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [x] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-10 12:35:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-cloud-agent/pull/1027" class=".btn">#1027</a>
            </td>
            <td>
                <b>
                    test: add tests for oid4vci credential configuration CRUD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">pollux</span><span class="chip">build</span><span class="chip">infra</span><span class="chip">shared</span><span class="chip">mercury</span><span class="chip">castor</span><span class="chip">cloud-agent</span>
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
        Created At 2024-05-10 08:34:11 +0000 UTC
    </div>
</div>

