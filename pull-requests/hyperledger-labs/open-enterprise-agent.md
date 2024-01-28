---
layout: default
title: open-enterprise-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/open-enterprise-agent
---

# open-enterprise-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/open-enterprise-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/867" class=".btn">#867</a>
            </td>
            <td>
                <b>
                    build: scala-steward dependency updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span><span class="chip">build</span><span class="chip">infra</span>
            </td>
            <td>
                ## About this PR
Updates:

* 📦 [ch.qos.logback:logback-classic](https://github.com/qos-ch/logback) from `1.4.8` to `1.4.14`
* 📦 [com.github.dasniko:testcontainers-keycloak](https://github.com/dasniko/testcontainers-keycloak) from `3.0.0` to `3.2.0`
  + 📜 [GitHub Release Notes](https://github.com/dasniko/testcontainers-keycloak/releases/tag/v3.2.0)
* 📦 [com.github.jwt-scala:jwt-circe](https://github.com/jwt-scala/jwt-scala) from `9.1.2` to `9.4.6`
  + 📜 [GitHub Release Notes](https://github.com/jwt-scala/jwt-scala/releases/tag/v9.4.6) - [Version Diff](https://github.com/jwt-scala/jwt-scala/compare/v9.1.2...v9.4.6)
* 📦 [com.github.poslegm:munit-zio](https://github.com/poslegm/munit-zio) from `0.1.1` to `0.2.0`
  + 📜 [GitHub Release Notes](https://github.com/poslegm/munit-zio/releases/tag/v0.2.0) - [Version Diff](https://github.com/poslegm/munit-zio/compare/v0.1.1...v0.2.0)
* 📦 [com.github.sbt:sbt-native-packager](https://github.com/sbt/sbt-native-packager) from `1.9.11` to `1.9.16`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-native-packager/releases/tag/v1.9.16) - [Changelog](https://github.com/sbt/sbt-native-packager/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/sbt/sbt-native-packager/compare/v1.9.11...v1.9.16)
* 📦 [com.github.sbt:sbt-release](https://github.com/sbt/sbt-release) from `1.1.0` to `1.4.0`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt-release/releases/tag/v1.4.0) - [Version Diff](https://github.com/sbt/sbt-release/compare/v1.1.0...v1.4.0)
* 📦 [com.networknt:json-schema-validator](https://github.com/networknt/json-schema-validator) from `1.0.86` to `1.0.88`
  + 📜 [GitHub Release Notes](https://github.com/networknt/json-schema-validator/releases/tag/1.0.88) - [Changelog](https://github.com/networknt/json-schema-validator/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/networknt/json-schema-validator/compare/1.0.86...1.0.88)
* 📦 [com.softwaremill.sttp.client3:zio-json](https://github.com/softwaremill/sttp) from `3.8.3` to `3.8.16`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-json/releases/tag/v0.6.2) - [Version Diff](https://github.com/zio/zio-json/compare/v0.3.0...v0.6.2)
* 📦 [com.softwaremill.sttp.tapir:tapir-http4s-server-zio](https://github.com/softwaremill/tapir) from `1.6.4` to `1.9.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.9.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.9.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-json-zio](https://github.com/softwaremill/tapir) from `1.6.4` to `1.9.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.9.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.9.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-prometheus-metrics](https://github.com/softwaremill/tapir) from `1.6.4` to `1.9.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.9.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.9.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-redoc-bundle](https://github.com/softwaremill/tapir) from `1.6.4` to `1.9.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.9.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.9.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-sttp-stub-server](https://github.com/softwaremill/tapir) from `1.6.4` to `1.9.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.9.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.9.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-swagger-ui-bundle](https://github.com/softwaremill/tapir) from `1.6.4` to `1.9.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.9.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.9.7)
* 📦 [com.softwaremill.sttp.tapir:tapir-zio-http-server](https://github.com/softwaremill/tapir) from `1.6.4` to `1.9.7`
  + 📜 [GitHub Release Notes](https://github.com/softwaremill/tapir/releases/tag/v1.9.7) - [Version Diff](https://github.com/softwaremill/tapir/compare/v1.6.4...v1.9.7)
* 📦 [com.thesamet:sbt-protoc](https://github.com/thesamet/sbt-protoc) from `1.0.6` to `1.0.7`
  + 📜 [GitHub Release Notes](https://github.com/thesamet/sbt-protoc/releases/tag/v1.0.7) - [Changelog](https://github.com/thesamet/sbt-protoc/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/thesamet/sbt-protoc/compare/v1.0.6...v1.0.7)
* 📦 [com.thesamet.scalapb:compilerplugin](https://github.com/scalapb/ScalaPB) from `0.11.13` to `0.11.15`
  + 📜 [GitHub Release Notes](https://github.com/scalapb/ScalaPB/releases/tag/v0.11.15) - [Changelog](https://github.com/scalapb/ScalaPB/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/scalapb/ScalaPB/compare/v0.11.13...v0.11.15)
* 📦 [com.thesamet.scalapb:scalapb-runtime-grpc](https://github.com/scalapb/ScalaPB) from `0.11.13` to `0.11.15`
  + 📜 [GitHub Release Notes](https://github.com/scalapb/ScalaPB/releases/tag/v0.11.15) - [Changelog](https://github.com/scalapb/ScalaPB/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/scalapb/ScalaPB/compare/v0.11.13...v0.11.15)
* 📦 [com.typesafe:config](https://github.com/lightbend/config) from `1.4.2` to `1.4.3`
  + 📜 [GitHub Release Notes](https://github.com/lightbend/config/releases/tag/v1.4.3) - [Version Diff](https://github.com/lightbend/config/compare/v1.4.2...v1.4.3)
* 📦 [dev.zio:zio](https://github.com/zio/zio) from `2.0.18` to `2.0.21`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.0.21) - [Version Diff](https://github.com/zio/zio/compare/v2.0.18...v2.0.21)
* 📦 [dev.zio:zio-concurrent](https://github.com/zio/zio) from `2.0.18` to `2.0.21`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.0.21) - [Version Diff](https://github.com/zio/zio/compare/v2.0.18...v2.0.21)
* 📦 [dev.zio:zio-config](https://github.com/zio/zio-config) from `3.0.7` to `4.0.1` ⚠
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-config/releases/tag/v4.0.1) - [Version Diff](https://github.com/zio/zio-config/compare/v3.0.7...v4.0.1)
* 📦 [dev.zio:zio-config-magnolia](https://github.com/zio/zio-config) from `3.0.7` to `4.0.1` ⚠
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-config/releases/tag/v4.0.1) - [Version Diff](https://github.com/zio/zio-config/compare/v3.0.7...v4.0.1)
* 📦 [dev.zio:zio-config-typesafe](https://github.com/zio/zio-config) from `3.0.7` to `4.0.1` ⚠
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-config/releases/tag/v4.0.1) - [Version Diff](https://github.com/zio/zio-config/compare/v3.0.7...v4.0.1)
* 📦 [dev.zio:zio-interop-cats](https://github.com/zio/interop-cats/) from `3.3.0` to `23.1.0.0`
  + 📜 [GitHub Release Notes](https://github.com/zio/interop-cats/releases/tag/v23.1.0.0) - [Version Diff](https://github.com/zio/interop-cats/compare/v3.3.0...v23.1.0.0)
* 📦 [dev.zio:zio-json](https://github.com/softwaremill/sttp) from `0.3.0` to `0.6.2`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-json/releases/tag/v0.6.2) - [Version Diff](https://github.com/zio/zio-json/compare/v0.3.0...v0.6.2)
* 📦 [dev.zio:zio-logging](https://github.com/zio/zio-logging) from `2.0.1` to `2.2.0`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-logging/releases/tag/v2.2.0) - [Version Diff](https://github.com/zio/zio-logging/compare/v2.0.1...v2.2.0)
* 📦 [dev.zio:zio-metrics-connectors-micrometer](https://github.com/zio/zio-metrics-connectors/) from `2.1.0` to `2.3.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-metrics-connectors/releases/tag/v2.3.1) - [Version Diff](https://github.com/zio/zio-metrics-connectors/compare/v2.1.0...v2.3.1)
* 📦 [dev.zio:zio-mock](https://github.com/zio/zio-mock) from `1.0.0-RC11` to `1.0.0-RC12`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-mock/releases/tag/v1.0.0-RC12) - [Version Diff](https://github.com/zio/zio-mock/compare/v1.0.0-RC11...v1.0.0-RC12)
* 📦 [dev.zio:zio-prelude](https://github.com/zio/zio-prelude) from `1.0.0-RC16` to `1.0.0-RC22`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-prelude/releases/tag/v1.0.0-RC22) - [Version Diff](https://github.com/zio/zio-prelude/compare/v1.0.0-RC16...v1.0.0-RC22)
* 📦 [dev.zio:zio-test](https://github.com/zio/zio) from `2.0.18` to `2.0.21`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.0.21) - [Version Diff](https://github.com/zio/zio/compare/v2.0.18...v2.0.21)
* 📦 [dev.zio:zio-test-magnolia](https://github.com/zio/zio) from `2.0.18` to `2.0.21`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.0.21) - [Version Diff](https://github.com/zio/zio/compare/v2.0.18...v2.0.21)
* 📦 [dev.zio:zio-test-sbt](https://github.com/zio/zio) from `2.0.18` to `2.0.21`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio/releases/tag/v2.0.21) - [Version Diff](https://github.com/zio/zio/compare/v2.0.18...v2.0.21)
* 📦 [io.getquill:quill-doobie](https://github.com/zio/zio-protoquill) from `4.7.3` to `4.8.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-protoquill/releases/tag/v4.8.1) - [Changelog](https://github.com/zio/zio-protoquill/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/zio/zio-protoquill/compare/v4.7.3...v4.8.1)
* 📦 [io.getquill:quill-jdbc-zio](https://github.com/zio/zio-protoquill) from `4.7.3` to `4.8.1`
  + 📜 [GitHub Release Notes](https://github.com/zio/zio-protoquill/releases/tag/v4.8.1) - [Changelog](https://github.com/zio/zio-protoquill/blob/master/CHANGELOG.md) - [Version Diff](https://github.com/zio/zio-protoquill/compare/v4.7.3...v4.8.1)
* 📦 [io.github.jopenlibs:vault-java-driver](https://github.com/jopenlibs/vault-java-driver) from `6.1.0` to `6.2.0`
  + 📜 [GitHub Release Notes](https://github.com/jopenlibs/vault-java-driver/releases/tag/v6.2.0) - [Version Diff](https://github.com/jopenlibs/vault-java-driver/compare/v6.1.0...v6.2.0)
* 📦 [io.micrometer:micrometer-core](https://github.com/micrometer-metrics/micrometer) from `1.11.2` to `1.11.8`
  + 📜 [GitHub Release Notes](https://github.com/micrometer-metrics/micrometer/releases/tag/v1.11.8) - [Version Diff](https://github.com/micrometer-metrics/micrometer/compare/v1.11.2...v1.11.8)
* 📦 [io.micrometer:micrometer-registry-prometheus](https://github.com/micrometer-metrics/micrometer) from `1.11.2` to `1.11.8`
  + 📜 [GitHub Release Notes](https://github.com/micrometer-metrics/micrometer/releases/tag/v1.11.8) - [Version Diff](https://github.com/micrometer-metrics/micrometer/compare/v1.11.2...v1.11.8)
* 📦 [net.reactivecore:circe-json-schema](https://github.com/reactivecore/rc-circe-json-schema) from `0.3.0` to `0.4.1`
  + 📜 [GitHub Release Notes](https://github.com/reactivecore/rc-circe-json-schema/releases/tag/v0.4.1) - [Version Diff](https://github.com/reactivecore/rc-circe-json-schema/compare/v0.3.0...v0.4.1)
* 📦 org.bouncycastle:bcpkix-jdk15on from `1.70` to `1.77`
* 📦 org.bouncycastle:bcprov-jdk15on from `1.70` to `1.77`
* 📦 [org.didcommx:didcomm](https://github.com/sicpa-dlab/didcomm-jvm) from `0.3.1` to `0.3.2`
  + 📜 [GitHub Release Notes](https://github.com/sicpa-dlab/didcomm-jvm/releases/tag/v0.3.2) - [Version Diff](https://github.com/sicpa-dlab/didcomm-jvm/compare/v0.3.1...v0.3.2)
* 📦 [org.didcommx:peerdid](https://github.com/sicpa-dlab/peer-did-jvm) from `0.3.0` to `0.4.1`
  + 📜 [GitHub Release Notes](https://github.com/sicpa-dlab/peer-did-jvm/releases/tag/v0.4.1) - [Version Diff](https://github.com/sicpa-dlab/peer-did-jvm/compare/v0.3.0...v0.4.1)
* 📦 [org.flywaydb:flyway-core](https://github.com/flyway/flyway) from `9.8.3` to `9.22.3`
* 📦 [org.http4s:http4s-blaze-server](https://github.com/http4s/blaze) from `0.23.12` to `0.23.16`
  + 📜 [GitHub Release Notes](https://github.com/http4s/blaze/releases/tag/v0.23.16) - [Version Diff](https://github.com/http4s/blaze/compare/v0.23.12...v0.23.16)
* 📦 org.keycloak:keycloak-authz-client from `22.0.4` to `22.0.5`
* 📦 [org.postgresql:postgresql](https://github.com/pgjdbc/pgjdbc) from `42.2.27` to `42.7.1`
  + 📜 [Changelog](https://github.com/pgjdbc/pgjdbc/blob/master/CHANGELOG.md)
* 📦 [org.scala-sbt:sbt](https://github.com/sbt/sbt) from `1.9.7` to `1.9.8`
  + 📜 [GitHub Release Notes](https://github.com/sbt/sbt/releases/tag/v1.9.8) - [Version Diff](https://github.com/sbt/sbt/compare/v1.9.7...v1.9.8)
* 📦 [org.scalameta:munit](https://github.com/scalameta/munit) from `1.0.0-M8` to `1.0.0-M10`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/munit/releases/tag/v1.0.0-M10) - [Version Diff](https://github.com/scalameta/munit/compare/v1.0.0-M8...v1.0.0-M10)
* 📦 [org.scalameta:sbt-scalafmt](https://github.com/scalameta/sbt-scalafmt) from `2.5.0` to `2.5.2`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/sbt-scalafmt/releases/tag/v2.5.2) - [Version Diff](https://github.com/scalameta/sbt-scalafmt/compare/v2.5.0...v2.5.2)
* 📦 [org.scalameta:scalafmt-core](https://github.com/scalameta/scalafmt) from `3.7.10` to `3.7.17`
  + 📜 [GitHub Release Notes](https://github.com/scalameta/scalafmt/releases/tag/v3.7.17) - [Version Diff](https://github.com/scalameta/scalafmt/compare/v3.7.10...v3.7.17)
* 📦 [org.scalatest:scalatest](https://github.com/scalatest/scalatest) from `3.2.16` to `3.2.17`
  + 📜 [GitHub Release Notes](https://github.com/scalatest/scalatest/releases/tag/release-3.2.17) - [Version Diff](https://github.com/scalatest/scalatest/compare/release-3.2.16...release-3.2.17)
* 📦 [org.scalatestplus:mockito-4-11](https://github.com/scalatest/scalatestplus-mockito) from `3.2.16.0` to `3.2.17.0`
* 📦 [org.scoverage:sbt-coveralls](https://github.com/scoverage/sbt-coveralls) from `1.3.9` to `1.3.11`
  + 📜 [GitHub Release Notes](https://github.com/scoverage/sbt-coveralls/releases/tag/v1.3.11) - [Version Diff](https://github.com/scoverage/sbt-coveralls/compare/v1.3.9...v1.3.11)
* 📦 [org.scoverage:sbt-scoverage](https://github.com/scoverage/sbt-scoverage) from `2.0.6` to `2.0.9`
  + 📜 [GitHub Release Notes](https://github.com/scoverage/sbt-scoverage/releases/tag/v2.0.9) - [Version Diff](https://github.com/scoverage/sbt-scoverage/compare/v2.0.6...v2.0.9)
* 📦 org.slf4j:slf4j-api from `2.0.7` to `2.0.11`
* 📦 org.slf4j:slf4j-simple from `2.0.7` to `2.0.11`
* 📦 [org.tpolecat:doobie-hikari](https://github.com/tpolecat/doobie) from `1.0.0-RC2` to `1.0.0-RC5`
  + 📜 [GitHub Release Notes](https://github.com/tpolecat/doobie/releases/tag/v1.0.0-RC5) - [Version Diff](https://github.com/tpolecat/doobie/compare/v1.0.0-RC2...v1.0.0-RC5)
* 📦 [org.tpolecat:doobie-postgres](https://github.com/tpolecat/doobie) from `1.0.0-RC2` to `1.0.0-RC5`
  + 📜 [GitHub Release Notes](https://github.com/tpolecat/doobie/releases/tag/v1.0.0-RC5) - [Version Diff](https://github.com/tpolecat/doobie/compare/v1.0.0-RC2...v1.0.0-RC5)

## Usage
✅ **Please merge!**

I'll automatically update this PR to resolve conflicts as long as you don't change it yourself.

If you have any feedback, just mention me in the comments below.

Configure Scala Steward for your repository with a [`.scala-steward.conf`](https://github.com/scala-steward-org/scala-steward/blob/33d3ad7d5245cbd05d7004d5502f6f7333833843/docs/repo-specific-configuration.md) file.

_Have a fantastic day writing Scala!_

<details>
<summary>🔍 Files still referring to the old version numbers</summary>

The following files still refer to the old version numbers.
You might want to review and update them manually.
```
DEPENDENCIES.md
build.sbt
docs/decisions/20220919-use-markdown-architectural-decision-records.md
package-lock.json
package.json
prism-agent/client/generator/yarn.lock
prism-agent/client/typescript/package.json
tests/performance-tests/atala-performance-tests-k6/yarn.lock
infrastructure/single-tenant-testing-stack/dashboards/oea-k6-detail.json
infrastructure/single-tenant-testing-stack/dashboards/oea-k8s-overview.json
CHANGELOG.md
docs/docusaurus/schemas/update.md
prism-agent/service/api/http/prism-agent-openapi-spec.yaml
prism-agent/service/server/src/main/scala/io/iohk/atala/system/controller/http/HealthInfo.scala
castor/lib/CHANGELOG.md
connect/lib/CHANGELOG.md
mercury/mercury-library/CHANGELOG.md
pollux/lib/CHANGELOG.md
prism-agent/service/CHANGELOG.md
prism-node/client/scala-client/CHANGELOG.md
shared/CHANGELOG.md
tests/integration-tests/build.gradle.kts
```
</details>
<details>
<summary>⚙ Adjust future updates</summary>

Add these to your `.scala-steward.conf` file to ignore future updates of these dependencies:
```
updates.ignore = [
  { groupId = "ch.qos.logback", artifactId = "logback-classic" },
  { groupId = "com.github.dasniko", artifactId = "testcontainers-keycloak" },
  { groupId = "com.github.jwt-scala", artifactId = "jwt-circe" },
  { groupId = "com.github.poslegm", artifactId = "munit-zio" },
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
  { groupId = "com.typesafe", artifactId = "config" },
  { groupId = "dev.zio", artifactId = "zio" },
  { groupId = "dev.zio", artifactId = "zio-concurrent" },
  { groupId = "dev.zio", artifactId = "zio-config" },
  { groupId = "dev.zio", artifactId = "zio-config-magnolia" },
  { groupId = "dev.zio", artifactId = "zio-config-typesafe" },
  { groupId = "dev.zio", artifactId = "zio-interop-cats" },
  { groupId = "dev.zio", artifactId = "zio-json" },
  { groupId = "dev.zio", artifactId = "zio-logging" },
  { groupId = "dev.zio", artifactId = "zio-metrics-connectors-micrometer" },
  { groupId = "dev.zio", artifactId = "zio-mock" },
  { groupId = "dev.zio", artifactId = "zio-prelude" },
  { groupId = "dev.zio", artifactId = "zio-test" },
  { groupId = "dev.zio", artifactId = "zio-test-magnolia" },
  { groupId = "dev.zio", artifactId = "zio-test-sbt" },
  { groupId = "io.getquill", artifactId = "quill-doobie" },
  { groupId = "io.getquill", artifactId = "quill-jdbc-zio" },
  { groupId = "io.github.jopenlibs", artifactId = "vault-java-driver" },
  { groupId = "io.micrometer", artifactId = "micrometer-core" },
  { groupId = "io.micrometer", artifactId = "micrometer-registry-prometheus" },
  { groupId = "net.reactivecore", artifactId = "circe-json-schema" },
  { groupId = "org.bouncycastle", artifactId = "bcpkix-jdk15on" },
  { groupId = "org.bouncycastle", artifactId = "bcprov-jdk15on" },
  { groupId = "org.didcommx", artifactId = "didcomm" },
  { groupId = "org.didcommx", artifactId = "peerdid" },
  { groupId = "org.flywaydb", artifactId = "flyway-core" },
  { groupId = "org.http4s", artifactId = "http4s-blaze-server" },
  { groupId = "org.keycloak", artifactId = "keycloak-authz-client" },
  { groupId = "org.postgresql", artifactId = "postgresql" },
  { groupId = "org.scala-sbt", artifactId = "sbt" },
  { groupId = "org.scalameta", artifactId = "munit" },
  { groupId = "org.scalameta", artifactId = "sbt-scalafmt" },
  { groupId = "org.scalameta", artifactId = "scalafmt-core" },
  { groupId = "org.scalatest", artifactId = "scalatest" },
  { groupId = "org.scalatestplus", artifactId = "mockito-4-11" },
  { groupId = "org.scoverage", artifactId = "sbt-coveralls" },
  { groupId = "org.scoverage", artifactId = "sbt-scoverage" },
  { groupId = "org.slf4j", artifactId = "slf4j-api" },
  { groupId = "org.slf4j", artifactId = "slf4j-simple" },
  { groupId = "org.tpolecat", artifactId = "doobie-hikari" },
  { groupId = "org.tpolecat", artifactId = "doobie-postgres" }
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
    dependency = { groupId = "com.github.dasniko", artifactId = "testcontainers-keycloak" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.github.jwt-scala", artifactId = "jwt-circe" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "com.github.poslegm", artifactId = "munit-zio" }
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
    dependency = { groupId = "com.typesafe", artifactId = "config" }
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
    dependency = { groupId = "dev.zio", artifactId = "zio-interop-cats" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-json" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-logging" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-metrics-connectors-micrometer" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "dev.zio", artifactId = "zio-mock" }
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
    dependency = { groupId = "io.github.jopenlibs", artifactId = "vault-java-driver" }
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
    dependency = { groupId = "net.reactivecore", artifactId = "circe-json-schema" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.bouncycastle", artifactId = "bcpkix-jdk15on" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.bouncycastle", artifactId = "bcprov-jdk15on" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.didcommx", artifactId = "didcomm" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.didcommx", artifactId = "peerdid" }
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
    dependency = { groupId = "org.keycloak", artifactId = "keycloak-authz-client" }
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
    dependency = { groupId = "org.scalameta", artifactId = "munit" }
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
    dependency = { groupId = "org.scalatestplus", artifactId = "mockito-4-11" }
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
    dependency = { groupId = "org.slf4j", artifactId = "slf4j-api" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.slf4j", artifactId = "slf4j-simple" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.tpolecat", artifactId = "doobie-hikari" }
  },
  {
    pullRequests = { frequency = "30 days" },
    dependency = { groupId = "org.tpolecat", artifactId = "doobie-postgres" }
  }
]
```
</details>

<sup>
labels: library-update, test-library-update, sbt-plugin-update, early-semver-patch, semver-spec-patch, early-semver-minor, semver-spec-minor, version-scheme:early-semver, early-semver-major, semver-spec-major, early-semver-pre-release, semver-spec-pre-release, version-scheme:always, artifact-migrations, old-version-remains, commit-count:n:43
</sup>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-28 01:10:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/865" class=".btn">#865</a>
            </td>
            <td>
                <b>
                    feat: add credential def performance test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">infra</span><span class="chip">ci</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-xxxx

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [ ] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 15:44:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/861" class=".btn">#861</a>
            </td>
            <td>
                <b>
                    docs: add description to credential definition and system endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-6274, ATL-6266

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [ ] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [x] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-24 12:48:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/860" class=".btn">#860</a>
            </td>
            <td>
                <b>
                    docs(prism-agent): update readme file to the latest Agent version, fix the broken link to the container registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">docs</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Resolves #858 and #838 

## Checklist

### My PR contains...
* [x] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [x] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [x] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 14:59:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/open-enterprise-agent/pull/855" class=".btn">#855</a>
            </td>
            <td>
                <b>
                    docs: improve oas doc for DID and wallet endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">prism-agent</span>
            </td>
            <td>
                # Overview
<!-- What this PR does, and why is needed, a useful description is expected, and relevant tickets should be mentioned -->

Fixes ATL-6270, ATL-6276

## Checklist

### My PR contains...
* [ ] No code changes (changes to documentation, CI, metadata, etc.)
* [ ] Bug fixes (non-breaking change which fixes an issue)
* [ ] Improvements (misc. changes to existing features)
* [ ] Features (non-breaking change which adds functionality)

### My changes...
* [ ] are breaking changes
* [ ] are not breaking changes
* [ ] If yes to above: I have updated the documentation accordingly

### Documentation
* [ ] My changes do not require a change to the project documentation
* [ ] My changes require a change to the project documentation
* [ ] If yes to above: I have updated the documentation accordingly

### Tests
* [ ] My changes can not or do not need to be tested
* [ ] My changes can and should be tested by unit and/or integration tests
* [ ] If yes to above: I have added tests to cover my changes
* [ ] If yes to above: I have taken care to cover edge cases in my tests

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 09:22:10 +0000 UTC
    </div>
</div>

