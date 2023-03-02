---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/993" class=".btn">#993</a>
            </td>
            <td>
                <b>
                    Fix go lint issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix go lint issue by running goimports.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 17:11:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/992" class=".btn">#992</a>
            </td>
            <td>
                <b>
                    Revert "Bump github.com/prometheus/client_golang from 1.1.0 to 1.11.1 in /high-throughput/application-go"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts hyperledger/fabric-samples#932
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 16:40:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/991" class=".btn">#991</a>
            </td>
            <td>
                <b>
                    Revert "Bump github.com/prometheus/client_golang from 1.1.0 to 1.11.1 in /asset-transfer-basic/application-go"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reverts hyperledger/fabric-samples#933
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 16:39:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/990" class=".btn">#990</a>
            </td>
            <td>
                <b>
                    Remove heritage chaincode samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The samples repository has been refactored to focus on an asset transfer series of samples. The goal of the samples repository is to align with the fabric documentation tutorials with minimal other distractions.
The heritage samples were left in place for a period of time until the asset transfer series stabilized. It is now time to purge the heritage samples.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 14:13:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/989" class=".btn">#989</a>
            </td>
            <td>
                <b>
                    Remove changelog script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Manual changelog is no longer created since github provides a changelog.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 14:02:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/961" class=".btn">#961</a>
            </td>
            <td>
                <b>
                    Fix gradle version used in asset-transfer-basic/chaincode-java image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch fixes the gradle version used in asset-transfer-basic/chaincode-java build to 7.

The reason is because the gradle version in the gradle:jdk11-alpine image is updated from 7 to 8, which seems to cause the build to fail. The result of running docker build command with gradle:jdk11-alpine are as follows:

```bash
Step 4/16 : RUN gradle --no-daemon build shadowJar -x checkstyleMain -x checkstyleTest
 ---> Running in d245170e621f

Welcome to Gradle 8.0.1!

Here are the highlights of this release:
 - Improvements to the Kotlin DSL
 - Fine-grained parallelism from the first build with configuration cache
 - Configurable Gradle user home cache cleanup

For more details see https://docs.gradle.org/8.0.1/release-notes.html

To honour the JVM settings for this build a single-use Daemon process will be forked. See https://docs.gradle.org/8.0.1/userguide/gradle_daemon.html#sec:disabling_the_daemon.
Daemon will be stopped at the end of the build 

FAILURE: Build failed with an exception.

* Where:
Build file '/home/gradle/build.gradle' line: 7

* What went wrong:
An exception occurred applying plugin request [id: 'application']
> Failed to apply plugin class 'com.github.jengelman.gradle.plugins.shadow.ShadowJavaPlugin'.
   > You can't map a property that does not exist: propertyName=classifier

* Try:
> Run with --stacktrace option to get the stack trace.
> Run with --info or --debug option to get more log output.
> Run with --scan to get full insights.

* Get more help at https://help.gradle.org

BUILD FAILED in 15s
The command '/bin/sh -c gradle --no-daemon build shadowJar -x checkstyleMain -x checkstyleTest' returned a non-zero code: 1

```

Related issues:
#940
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-24 00:44:18 +0000 UTC
    </div>
</div>

