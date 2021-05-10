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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/913" class=".btn">#913</a>
            </td>
            <td>
                <b>
                    refactor(core-api): get is replaced with post
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Core_API</span><span class="chip">dependent</span>
            </td>
            <td>
                Resolve #430 
Depends on #915 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 15:43:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/910" class=".btn">#910</a>
            </td>
            <td>
                <b>
                    feat(connector-quorum): support v21.4.1 and Tessera 21.1.1 #901
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Quorum</span><span class="chip">enhancement</span>
            </td>
            <td>
                Refactored how tests are named so that we can start having a support
matrix backed by tests for each permutation needed.

The used Quorum version is encoded in the beginning of the
test case file name to make them easy to tell apart in logs.

Fixes https://github.com/hyperledger/cactus/issues/901

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 22:58:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/909" class=".btn">#909</a>
            </td>
            <td>
                <b>
                    feat(test-tooling): quorum AIO upgrade to Quorum v21.4.1 #900
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">Quorum</span><span class="chip">dependencies</span><span class="chip">enhancement</span>
            </td>
            <td>
                The image will now have the currently latest & greatest from both
Quorum and Tessera.

This commit is also tagged in DockerHub as
hyperledger/cactus-quorum-all-in-one:2021-05-03-quorum-v21.4.1

Two minor updates that were necessary for the upgrade:
1. The allowing of unlocking while HTTP is enabled is now prohibited by default unless you pass
in a specific flag when starting Quorum (so we do).
2. The max code size schema has changed in the genesis file to include
block size as well so the genesis.json used is updated too.

Fixes https://github.com/hyperledger/cactus/issues/900

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 22:55:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/908" class=".btn">#908</a>
            </td>
            <td>
                <b>
                    refactor(test-tooling): quorum AIO supervisord to log to stdout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">Quorum</span>
            </td>
            <td>
                This makes it much easier to debug issues with the AIO container at runtime because
one does not have to shell into the container, find the log files manually and
then print them there. Instead the container just forwards the
output of Tessera and Quorum straight to it's own stdout/stderr.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 22:51:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/907" class=".btn">#907</a>
            </td>
            <td>
                <b>
                    feat(test-tooling): quorum test ledger omit pull parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">Quorum</span><span class="chip">dependencies</span><span class="chip">enhancement</span>
            </td>
            <td>
                With this boolean argument of the start() method of the test ledger
class one can test locally built container images that were no yet
pushed to a public docker registry.
To use it: build your docker image locally with a tag of "your-tag", then
specify this as the tag to be used and also the omitPull argument of the start
method as true which will result in your local image being used without
any attempts to pull it (which would fail).

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 22:34:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/906" class=".btn">#906</a>
            </td>
            <td>
                <b>
                    perf(cmd-api-server): shrink API server bundle with type-only imports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">Developer_Experience</span><span class="chip">dependencies</span><span class="chip">enhancement</span>
            </td>
            <td>
                Great explanation can be found here:
https://www.typescriptlang.org/docs/handbook/release-notes/typescript-3-8.html

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 21:03:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/905" class=".btn">#905</a>
            </td>
            <td>
                <b>
                    feat: besu WatchBlocksV1Endpoint with SocketIO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">dependencies</span><span class="chip">enhancement</span>
            </td>
            <td>
                ## Dependencies

Depends on [feat(cmd-api-server): add Socket.IO as transport #297 #897](#897)

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: 2021-05-03 09:52:27 -0700
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: 2021-05-03 13:16:52 -0700 

feat: besu WatchBlocksV1Endpoint with SocketIO

Primary change(s):
-----------------

1. Adds an async endpoint based on
the new SocketIO integration of the API server. The endpoint streams new
block headers to the clients as they come in through the subscription
mechanism of Web3.

2. The besu connector plugin is now capable of
accepting the WS RPC API host of the backing Besu client/ledger so that
it can instantiate a WebSocket provider for itself which was a
prerequisite of being able to use the Web3 subscriptions functionality
that the async endponit needs to work.

Secondary change(s):
-------------------

1. Updated the supply chain app example and the besu tests to
accomodate the change that the besu connector now needs to use
the web socket RPC API instead of the HTTP one.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 20:30:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/903" class=".btn">#903</a>
            </td>
            <td>
                <b>
                    refactor(core-api): register web service method to accept socket io srv
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">Core_API</span><span class="chip">enhancement</span>
            </td>
            <td>
                Adds a second parameter after the epxress object. The second parameter
is a SocketIO server object which plugins will be able to use to
register their asynchronous/streaming endpoints which do not use
traditional REST nor necessarily HTTP as the transport (think websocket
or SocketIO)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

Related to #297 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 20:14:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/902" class=".btn">#902</a>
            </td>
            <td>
                <b>
                    feat(core-api): add SocketIoConnectionPathV1 constant to OpenAPI specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Core_API</span>
            </td>
            <td>
                This defines a constant in the OpenAPI specification so that it can be
reused everywhere else in the code, including in the generated
documentation that we intend to create from the OpenAPI specifications
later on and also other packages in the Typescript code who import the
core-api package.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

Related to #297
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 20:09:47 +0000 UTC
    </div>
</div>

