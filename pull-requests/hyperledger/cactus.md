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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/894" class=".btn">#894</a>
            </td>
            <td>
                <b>
                    chore(linter): fix warning in isIPluginWebService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 21:24:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/892" class=".btn">#892</a>
            </td>
            <td>
                <b>
                    fix(github/workflows): dependent issues job name typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                There was a typo in the first fix I attempted so now fixing the fix here
(hopefully)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 21:13:20 +0000 UTC
    </div>
</div>

