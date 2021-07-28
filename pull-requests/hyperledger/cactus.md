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
                PR <a href="https://github.com/hyperledger/cactus/pull/1174" class=".btn">#1174</a>
            </td>
            <td>
                <b>
                    feat(examples/discounted_cartrade): add preferredcustomer-jugdement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yasushi Takahashi <t-yasushi@fujitsu.com>

resolves #1148 (update by Peter)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-28 02:52:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    refactor(core-api): keychain plugin get/set generics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #478
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 20:15:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1169" class=".btn">#1169</a>
            </td>
            <td>
                <b>
                    Draft pull request for Iroha connector plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 15:56:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    feat(besu): Support for private transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Support for besu private transactions is now enabled, this is done by adding privateFor and privateFrom fields in the HTTP request.

fixes #952 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 11:48:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1167" class=".btn">#1167</a>
            </td>
            <td>
                <b>
                    feat(corda): support release 4.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #888 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 13:52:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1166" class=".btn">#1166</a>
            </td>
            <td>
                <b>
                    build(deps): fix sync-npm-deps-to-tsc-projects tool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span>
            </td>
            <td>
                1. The ./tools/sync-npm-deps-to-tsc-projects.ts script
had a missing part in it which would fill the root
tsconfig.json file with the references to the packages
of the monorepo.

2. Point 1 could not be achieved without removing the
cactus-cockpit package from the dependencies of
cmd-api-server because the script mentioned above fails
if there are dependencies declared which do not exist
on the file-system anymore (which is exactly what
happened when we deprecated the cockpit package and then
forgot to remove it from the list of dependencies.

3. All the tsconfig.json files are updated by the sync
script (from point 1.)

4. Adds skip lib check true to the ipfs package's tsconfig
file so that the issue with uint8array dependency's own typings
don't break the build. For reference, the errors look like this:

- Error: node_modules/uint8arrays/dist/to-string.d.ts(20,24): error TS2307:
  Cannot find module './util/bases' or its corresponding type declarations.

- Error: node_modules/uint8arrays/dist/to-string.d.ts(21,34): error TS2307:
  Cannot find module './util/bases' or its corresponding type declarations.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 02:03:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1165" class=".btn">#1165</a>
            </td>
            <td>
                <b>
                    build: use yarn 1.19.0 instead of 1.22.10
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">dependencies</span>
            </td>
            <td>
                Needed to downgrade because of a bug in 1.22.10 where it was
unable to install dependencies into workspaces individually.

See details here: https://github.com/yarnpkg/yarn/issues/8405

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 01:05:26 +0000 UTC
    </div>
</div>

