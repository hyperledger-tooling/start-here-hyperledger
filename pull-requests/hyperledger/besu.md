---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3816" class=".btn">#3816</a>
            </td>
            <td>
                <b>
                    Fix for multi-arch docker develop and latest tags 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
## PR description

In the multi-arch docker build pr #2954, the manifest step is not correctly creating the `develop` and `latest` multi-arch tags.  This pr fixes the tag creation in the manifestDocker step

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 04:50:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3815" class=".btn">#3815</a>
            </td>
            <td>
                <b>
                    Migrate integrationTests to Junit5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
As an effort to modularize Junit5 migration, this PR only migrates tests ran from the `integrationTest` task.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 00:46:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3814" class=".btn">#3814</a>
            </td>
            <td>
                <b>
                    Replace expected Junit 4 @Test field with assertThatThrownBy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
To simplify a future Junit5 migration this PR removes the usage of the [expected](https://junit.org/junit4/javadoc/4.13/org/junit/Test.html#expected()) field of the `org.junit.Test` annotation with the AssertJ's `assertThatThrownBy` method.

- [HEAD~3](https://github.com/diega/besu/commit/expected_replace~3): Fix two tests from `o.h.b.e.vm.OperandStackTest`, the name of the tests referred to testing `o.h.b.e.internal.OperandStack#set` but they were actually testing _get_ (duplicated indeed, b/c proper tests for _get_ existed with the right method name) -> Thanks @macfarla!
- [HEAD~2](https://github.com/diega/besu/commit/expected_replace~2): Remove unreachable asserts
- [HEAD~1](https://github.com/diega/besu/commit/expected_replace~1): Syntactic wrapping of lines throwing the expected exception
- [HEAD](https://github.com/diega/besu/commit/expected_replace): Extract variables to let only a single method call inside the `assertThatThrownBy` lambda

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-10 22:54:47 +0000 UTC
    </div>
</div>

