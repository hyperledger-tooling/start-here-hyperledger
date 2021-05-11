---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): config-service example - authorization JSON
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">bug</span>
            </td>
            <td>
                The custom formatter that was introduced the parse the JSON
config for the authorizer was causing problems.
This was overlooked at the time of the implementation of the authz
feature because Peter (yours truly) is an idiot but also to a smaller
extent because there was no automated test coverage for this specific
issue which this commit is now rectifying by adding a new test case.

Longer term we should look into using a different configuration
parsing library that has more flexibility on how to handle JSON
and validations around it.

There was a second bug masked by the first which is that the
"algorithms" array property of the express-jwt middleware
options was also not being used correctly, but to get to that
first the initial bug with the parsing had to be fixed.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 18:15:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    fix(connector-besu): removed repeated check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">dependent</span>
            </td>
            <td>
                Resolve #882 
Depends on #915 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 14:44:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/919" class=".btn">#919</a>
            </td>
            <td>
                <b>
                    JDK replaced by docker openapitool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                Resolve #463 
Depends on #915
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 09:49:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/918" class=".btn">#918</a>
            </td>
            <td>
                <b>
                    refactor(supply-chain-backend): .test.ts suffix for api-surface tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                A cosmetic change that helps people identify whata re test files and are
main source files since Visual Studio Code has this feature
that it highlights .test.ts files with a different icon in its
file explorer.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 00:09:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/917" class=".btn">#917</a>
            </td>
            <td>
                <b>
                    refactor(core-api): discontinue the PluginAspect enum #885
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Core_API</span>
            </td>
            <td>
                Also fixed a few typos here and there, linter warnings, etc.

Fixes #885

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

cc: @AzaharaC @kikoncuo @jagpreetsinghsasan @TonyRowntree @travis-payne 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 23:57:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/915" class=".btn">#915</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): fix module requires Go 1.17 #914
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">bug</span><span class="chip">dependencies</span>
            </td>
            <td>
                Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Date: Tue May 04 2021 14:32:33 GMT-0700 (Pacific Daylight Time)	 

test(connector-fabric): fix module requires Go 1.17 #914

Primary change:
------------------

Pinned the buggy dependency to yesterday's version
(the bug was introduced in this morning's build).

This prevents today's version from being used and
fixes the problem.

Secondary change:
--------------------

Upgraded the container image that's being used for the test to
the one that has the fabric images pre-cached.
This leads to faster test execution and lower probability
of developers getting hit by the dreaded DockerHub rate limiting issue.

Fixes #914 

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 21:34:56 +0000 UTC
    </div>
</div>

