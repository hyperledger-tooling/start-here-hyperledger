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
                PR <a href="https://github.com/hyperledger/cactus/pull/1234" class=".btn">#1234</a>
            </td>
            <td>
                <b>
                    test: adding quorum multip test ledger Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This code allows for building of the a quorum multi party docker image that allows for private transactions to be tested.


Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 10:23:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1232" class=".btn">#1232</a>
            </td>
            <td>
                <b>
                    chore(deps): project-wide upgrade August, 2021
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">SPIKE</span><span class="chip">dependencies</span>
            </td>
            <td>
                Dependencies that were NOT upgraded to the latest:
1. jose
2. express-openapi-validator
3. prettier

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 04:46:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1230" class=".btn">#1230</a>
            </td>
            <td>
                <b>
                    chore(release): publish v0.8.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-17 03:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1229" class=".btn">#1229</a>
            </td>
            <td>
                <b>
                    refactor(cmd-api-server): migrate container to ubuntu-20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">dependencies</span>
            </td>
            <td>
                1. Makes the base image of the API server ubuntu-20.04
2. Upgrades the NodeJS version to v16

Published a version of this commit to ghcr as well, built it 
with this command:

DOCKER_BUILDKIT=1 docker build \
  --build-arg NPM_PKG_VERSION=fix-1226 \
  -f ./packages/cactus-cmd-api-server/Dockerfile . \
  -t cas \
  -t cactus-api-server

Tagged as:
ghcr.io/hyperledger/cactus-cmd-api-server:2021-08-15--refactor-1222

Fixes #1222

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 05:33:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1228" class=".btn">#1228</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): add missing deps remove unused ones #1226
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">API_Server</span><span class="chip">dependencies</span>
            </td>
            <td>
                Fixes #1226

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 04:53:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1225" class=".btn">#1225</a>
            </td>
            <td>
                <b>
                    fix(examples): front-end packages missing browserify polyfills #1224
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                The webpack build done by the Angular CLI (ng) was broken due to a few
different issues combined together:
1. After upgrading to Angular v12 IE 11 is no longer supported which
necessitated the explicit configuration in the browserlist rc config
file accordingly so that the compilation process does not try to support
a browser for which the build is broken to begin with.
2. polyfills had to be added via customizing the webpack configuration
used by the Angular CLI internally which is now being done by using a
custom builder as specified in the angular.json file. This is the new
method of dealing with these kind of issues after the ng eject command
was deprecated a while back. The webpack.config.overrides.js files
that are beind added in this commit contain only the overrides (as the
name suggests) not the entire webpack configuration that the Angular
CLI uses internally to build the front end packages.

Fixes #1224

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-16 02:39:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1221" class=".btn">#1221</a>
            </td>
            <td>
                <b>
                    test: ensure .test suffix on mTLS tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                These are likely the last test files that we have forgotten to
refactor to have a .test suffix which improves developer experience
on account of IDE support and easier filtering of files.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-14 03:56:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1220" class=".btn">#1220</a>
            </td>
            <td>
                <b>
                    ci: remove retries from ci.sh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The tests are still not 100% stable, but a lot more stable and
the retries might not be needed anymore.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-14 03:44:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1219" class=".btn">#1219</a>
            </td>
            <td>
                <b>
                    test(tools): besu multi-party AIO container image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">Besu</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Works with a modified (forked) version of quorum-dev-quickstart
See https://github.com/ConsenSys/quorum-dev-quickstart/pull/72

On the fork we added an extra commit that removes the usage of
tput (which is a low impact change because all
it is being used for is to make text in the terminal bold for cosmetic
purposes).

This is published on the public registry as:
ghcr.io/hyperledger/cactus-besu-all-in-one-multi-party:2021-08-13--private-tx

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-13 23:42:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1209" class=".btn">#1209</a>
            </td>
            <td>
                <b>
                    feat(ci): support debugging on CI server through ssh #717
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #717
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-12 14:15:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1206" class=".btn">#1206</a>
            </td>
            <td>
                <b>
                    Feat 1010 keychain azure handler endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 14:31:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1205" class=".btn">#1205</a>
            </td>
            <td>
                <b>
                    test(cmd-api-server): randomize port in config service test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">API_Server</span>
            </td>
            <td>
                If you don't specify port zero for the API and the cockpit then they
will default to 3000 and 4000 instead which is bad for
parallel test execution where we need guarantees not to
use potentially conflicting port numbers.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 04:38:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1204" class=".btn">#1204</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): plugins interfere with API server deps #1192
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">API_Server</span><span class="chip">dependencies</span><span class="chip">Security</span>
            </td>
            <td>
                Migrates to the lmify package to install plugins at runtime
instead of doing it via vanilla npm which was causing problems
with conflicting dependency versions where the API server would
want semver 7.x and one of the plugins (through some transient
dependency of the plugin itself) would install semver 5.x which
would then cause the API server to break down at runtime due to
the breaking changes between semver 7 and 5.

The magic sauce is the --prefix option of npm which, when specified
instructs npm to ignore the usual parent directory traversal algorithm
when evaluating/resolving dependency trees and instead just do a full
installation to the specified directory path as dictated by the
--prefix option. This means that we can install each plugin in their
own directory the code being isolated from the API server and also
from other plugins that might also interfere.

Fixes hyperledger#1192

Depends on hyperledger#1203

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 00:28:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1203" class=".btn">#1203</a>
            </td>
            <td>
                <b>
                    fix(prometheus): metrics.ts leaks to global registry #1202
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                fix(prometheus): metrics.ts leaks to global registry #1202
    
1. Specified a `register` property of the gauges as an empty
array so that it does not pollute the global namespace. This
is how this is supposed to be done as per the docs of prom-client.

2. Once the change from 1) took place, the issue became that
the metrics gathering code was still trying to hit up the
global scope for the metrics, e.g. calling the get metrics
methods directly on the promClient object instead of the
registry that we create for each prmoetheus exporter object
separately. So a little additional refactor ensued to fix this
as well by making sure that we grab a reference of the registry
object at construction time and then re-use that wherever needed
instead of going through the global promClient object.

3. Added missing .startMetricsCollection calls in the plugin
constructors to ensure that the prometheus exporter object
gets initialized properly (this is where the registry gets
created as well so without this there are crashes happening
when one tries to access the metrics through the registry)

Why though?
The problem was that the metrics.ts file that we have for all the
plugin's metrics constructs a new Metric (Gauge) object at import
time which then defaults to registering the metric in the global
registry of prom-client by default.

The latter was causing crashes when separate versions of the same
metrics.ts file are imported in a scenario were the API server
imports plugins from a different directory (this issue is coming
from the branch where I'm working on plugin sandboxing via the
live-plugin-manager).
    
Fixes #1202

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 22:34:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1201" class=".btn">#1201</a>
            </td>
            <td>
                <b>
                    fix(plugin-consortium-manual): drop repo constructor arg #1199
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Removes the non-serializable consortiumRepo argument from the
constructor of the consortium plugin manual class's options.

Refactors the constructor and the internals of the plugin  to initialize
the consortium repo from the consortium database at runtime
instead of expecting it passed in via the constructor.
Refactors the internal code previously using the options.consoritumRepo
object to use this.repo instead which is what gets initalized in
the constructor as explained above.

All this leads to equivalent functionality but less boilerplate and now
thanks to this the plugin can be (should be - more tests needed)
initialized by the API server purely based on the static configuration
file when necessary.

Fixes #1199

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 19:54:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1198" class=".btn">#1198</a>
            </td>
            <td>
                <b>
                    refactor(plugin-registry): getOneById to use instanceId #1197
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                The getOneById function will now use the instance ID
for lookups instead of the package name.

Also added a couple of extra convenience methods to make
them more consistent in general and increased the
test coverage of the plugin registry.

Fixes #1197

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 18:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1196" class=".btn">#1196</a>
            </td>
            <td>
                <b>
                    refactor(core-api): make schema names consistent in openapi spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1195

Signed-off-by: Youngone Lee <youngone.lee@accenture.com> 

@petermetz pinged for review! 
I have a few comments/questions regarding this issue: 

1. I should update this PR so that we also change the names for "get" and "set" to contain "V1"?
2. Could you take a look at the descriptions within the files and suggest what to write? 

Thank you ⭐!! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 17:39:08 +0000 UTC
    </div>
</div>

