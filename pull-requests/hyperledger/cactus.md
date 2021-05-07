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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/899" class=".btn">#899</a>
            </td>
            <td>
                <b>
                    feat: expose besu test ledger web socket API port
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">enhancement</span>
            </td>
            <td>
                Provide a method to retrieve the host port of the web socket JSON RPC
API exposed by the Besu AIO image backing the BesuTestLedger class. This
is a precursor to us adding support for the websocket transport in one
way or another (SocketIO != WebSockets in the strict sense of protocol
compatibility because SocketIO servers cannot be used by vanilla WS
applications out of the box)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/898" class=".btn">#898</a>
            </td>
            <td>
                <b>
                    perf: leverage import type syntax to save on bundle size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Core_API</span><span class="chip">Performance</span><span class="chip">dependent</span>
            </td>
            <td>
                ## Dependencies

Depends on #897 

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: 2021-05-01 16:49:48 -0700
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: 2021-05-01 17:13:43 -0700 

perf: leverage import type syntax to save on bundle size

We can exclude ExpressJS from the core-api bundles because it is
designed to only ship interfaces for re-use by other packages.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:18:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/897" class=".btn">#897</a>
            </td>
            <td>
                <b>
                    feat(cmd-api-server): add Socket.IO as transport #297
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">ConnectionChain</span><span class="chip">Core_API</span><span class="chip">dependent</span><span class="chip">enhancement</span>
            </td>
            <td>
                ## Dependencies

Depends on #896 
Depends on #899
Depends on #902
Depends on #903

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: 2021-05-03 09:20:49 -0700
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: 2021-05-03 09:39:40 -0700 

feat(cmd-api-server): add Socket.IO as transport #297

Primary changes:
---------------

1. The API server now has a SocketIO server running on the same port
as the HTTP REST API.

2. The API server now has an ApiServerApiClient class which is an
extension of the DefaultApi class that we generate from the OpenAPI
specifications. The reason why this extension was necessary (something
that we try to avoid like the plague normally) is because OpenAPI is
strictly for defining HTTP/REST based APIs and not async/streaming
ones such as WebSocket/SocketIO based ones and therefore the OpenAPI
generator does not support these types of transports at all meaning
that we have to manually write the client code for async endpoints
which is why the class extension here is not something that we can
get around.

3. The idea is that all async endpoints would declare their event
names as constants in the OpenAPI specification so as to make it
easier at least to some degree to implement solutions on top even
if we cannot support async endpoints with the OpenAPI code
generator to the same extend we do for HTTP RESTful endpoints.
The five default events are Subscribe, Next, Unsubscribe, Error and
Complete. These are defined in order to match what the client can
do on the RxJS Observable object returned by the API client object's
method that invokes the async endpoints.
The difference between Unsubscribe and complete is subtle, but it definitely
exists. The unsubscribe event is used by the client to tell the backend
that it no longer requires updates, regardless of the streaming of data
having been completed or not.
The complete event on the other hand is for the backend to signal that
the streaming of data is in fact completed. The complete event is only
applicable for endpoints that do have an ending which is not the case
for some endpoints that are usually time-series related and therefore
a lot of times just stream endlessly until stopped.

Secondary change(s):
--------------------

1. Added an async endpoint powered by the just now added SocketIO
integration that streams the health check response every one second
which is mainly added to that we can test the functionality but at
could also be used for monitoring purposes by someone who'd rather
implement something from scratch than use Prometheus for example.

To-do:
------

1. Socket provider singleton on client side for connection multiplexing

Fixes #297

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/896" class=".btn">#896</a>
            </td>
            <td>
                <b>
                    build: webpack ts-loader transpileOnly set to true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Needed this because otherwise the perfectly valid Typescript code would
not compile when using TS loader in cases when multiple Cactus packages
were depending on types from certain dependencies (example both core-api
and the besu connector would depend on the socketio package and its
"Server" class would be claimed as incompatible by the TS loader
compilation process even when the source files for those types were byte
to byte the same (but the path was different to them because they
existed in different node_modules directories)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:10:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/895" class=".btn">#895</a>
            </td>
            <td>
                <b>
                    build: remove npm dep. commitizen to avoid git-cz conflict
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allegedly fixes the strange git-cz error encountered
while running "npm run commit"

(node:11594) UnhandledPromiseRejectionWarning: TypeError: Cannot convert undefined or null to object
    at Function.keys (<anonymous>)
    at runInteractiveQuestions (//node_modules/git-cz/dist/cz.js:576:10)
    at run (//node_modules/git-cz/dist/cz.js:157:11)
    at exports.prompter (//node_modules/git-cz/dist/cz.js:164:3)
    at //node_modules/commitizen/dist/commitizen/commit.js:598:9
    at //node_modules/fs-extra/lib/mkdirs/mkdirs.js:56:16
    at callback (//node_modules/graceful-fs/polyfills.js:295:20)
    at FSReqCallback.oncomplete (fs.js:184:5)

Hit the same issue, multiple times with it disappearing and then resurfacing with different versions as well, made no sense.

So, I started checking other things and found out that I also had commitizen installed which for some reason declares it's own, conflicting binary also called git-cz that (I'm guessing) may end up being hooked up to ./node_modules/.bin/git-cz randomly depending on the cookie crumbles when you run npm install (which I assume does as much as possible parallelized)

Uninstalled commitizen and right now it's working. Just a theory, but maybe it's right.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>


cc: @travis-payne @TonyRowntree 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-02 00:08:18 +0000 UTC
    </div>
</div>

