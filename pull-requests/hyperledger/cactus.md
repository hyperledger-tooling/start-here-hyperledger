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
                <span class="chip">bug</span><span class="chip">API_Server</span><span class="chip">dependencies</span><span class="chip">Security</span><span class="chip">dependent</span>
            </td>
            <td>
                # 1 Commit to review (ignore the other one which is needed for tests to pass but is on another PR):

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Date:   Tue Aug 10 16:42:09 2021 -0700    
    
fix(cmd-api-server): plugins interfere with API server deps #1192

Migrates to the live-plugin-manager package to install plugins
instead of doing it via vanilla npm which was causing problems
with conflicting dependency versions where the API server would
want semver 7.x and one of the plugins (through some transient
dependency of the plugin itself) would install semver 5.x which
would then cause the API server to break down at runtime due to
the breaking changes between semver 7 and 5.

The hope with the new live-plugin-manager package is that using
this will provide sufficient isolation so that these kind of issues
are non-existent and also that it does not introduce other different
types of issues stemming from exactly said isolation. With that said
if isolation problems do occur we'll have to fix that anyway because
the plugins should not depend on the API server and vica versa.

Fixes #1192

Depends on #1203

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

1. I should update this PR so that we also change the names for "get" and "set" to contain?
2. Could you take a look at the descriptions within the files and suggest what to write? 

Thank you ⭐!! 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 17:39:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1193" class=".btn">#1193</a>
            </td>
            <td>
                <b>
                    refactor: remap ts typings from types to lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was necessary because if we import JSON files and
then re-use their schema as types, then the d.ts files
will need to have access to said JSON file which does
not happen if the typings and the actual .js code are
in separate directories because then the relative paths
are not working as they should.

Moving the lib and the types together means that now
the d.ts files can import with the same relative paths
that the orignial source code (.ts files) can as well.

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 21:03:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1191" class=".btn">#1191</a>
            </td>
            <td>
                <b>
                    feat(connector-quorum): remove hard dependency on keychain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                feat(quorum): remove hard dependency on keychain

Removed hard dependency on keychain for Quorum plugin.

Updated old test cases and added new test cases.

resolves #1161 

Signed-off-by: TonyRowntree <33454202+TonyRowntree@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 12:48:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    feat(cmd-api-server): support grpc web services #1189
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">API_Server</span>
            </td>
            <td>
                # WORK IN PROGRESS

Fixes #1189
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 06:38:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1188" class=".btn">#1188</a>
            </td>
            <td>
                <b>
                    feat(keychain-google-sm): complete request handler and endpoints #1097
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                Fixes #1097 

Depends on #1196
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 19:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1187" class=".btn">#1187</a>
            </td>
            <td>
                <b>
                    fix(example): send http request to discounted-cartrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This resolve Issue #1181 
I create req_discounted_cartrade.py in example/discounted-cartrade.
This sends http request to discounted-cartrade after resistors indy data.

Signed-off-by: Yasushi Takahashi <t-yasushi@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-06 06:46:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    chore(release): publish v0.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 21:30:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    build(package.json): add reset script that git cleans prior to configure
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Why though?
This is designed to eliminate possible build issues that arise because of leftover code files
somehow lurking around the project directory structure that are being ignored by git and
therefore lulling a contributor to thinking that since VSCode shows no index/staged changes
the project is in a clean slate and the build should pass all the same.
The reset script in essence is a softer version of going all out, deleting your entire
project directory and cloning it from scratch which is a lot more effort than just running
the reset script added here that has a good chance of fixing the same problems as the hard
resetting if re-clone would fix.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 19:02:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1184" class=".btn">#1184</a>
            </td>
            <td>
                <b>
                    build: yarnrc --ignore-engines true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">Developer_Experience</span>
            </td>
            <td>
                Specifies the --ignore-engines true parameter to be the default for
every yarn command contributors run within the project. This makes it
sligthly more convenient to work with yarn since now you can just say
"yarn install" instead of having to go with the much longer "yarn
install --ignore-engines". 

Of course in an ideal world we would not need
the --ignore-engines parameter but the Fabric Node SDK (and some other
dependencies probably) do not declare NodeJS v16 as a supported engine
(despite our tests succeeding on these) so we just do not have a choice
with this if we want to support NodeJS 16 (which we very much
do)

Also removes --ignore-engines parameter from the yarn install
command that the configure script runs so that the CI also verifies this
to be working fine.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-04 05:10:42 +0000 UTC
    </div>
</div>

