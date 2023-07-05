---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2535" class=".btn">#2535</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add new connector plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add new plugin for connecting with Ethereum ledgers. New connector is based on already existing quorum connector. The main reason for introducing yet another plugin is a need for web3js upgrade (to 4.X) which is imposible in current quorum / besu connectors due to dependency to `web3js-quorum` which requires web3js 1.X.

We have plans to make web3js library pluggable and reduce code duplication among other connectors in the future, but it will be delivered later on in a separate PR.

Changes:
- Add new plugin based on quorum connector.
- Removed private transaction and other quorum related functionalities.
- Update web3js to 1.10 - will be updated to 4.X in a separate commit.
- Add missing `web3-eth-contract` dependencies to besu and xdai connectors.
- Add new connector to cactus-verifier-client
- Add integration tests in `cactus-test-plugin-ledger-connector-ethereum` (based on similar ones for quorum connector.)
- Add new connector to CI.
- Add `web3*` 1.5.2 dependencies to root `package.json` because they are already required in a root level (by `typings/web3js-quorum`). Ideally this could be put into another package (quorum connector?) and have the dependencies there, but for now I think it's important to be explicit about it since it's easy to mess up if wrong web3js library is hoisted up from any monorepo package.
- Sort main `package.json`
- Remove tap test scripts from the root `package.json` - they don't use `.taprc` and cause bunch of errors when they try to execute jest tests. This is confusing for the users because of all false negative errors printed.
- Reorganize jest config and taprc to keep tests from quorum and ethereum conenctors grouped.

Closes: #2534
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 15:17:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2533" class=".btn">#2533</a>
            </td>
            <td>
                <b>
                    fix(weaver-corda): throw error correctly in responder flows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bug fix in corda interop app (weaver), where flows would get stuck if responder flow verification fails.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 18:58:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2530" class=".btn">#2530</a>
            </td>
            <td>
                <b>
                    docs(examples): upgrade Angular to v14
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Upgraded Angular from v13 to v14
2. Also bumped up the Ionic Framework dependencies
as needed because older versions that we were using
were not compatible [1] with Angular v14
3. Also did some of the Cactus -> Cacti renaming
in the front-end code namely the front-page of
both the supply chain and the carbon accounting
app examples.

[1] https://stackoverflow.com/a/72508644

Verbatim copy of the above link's comment:

==================================
The current version of Ionic v6.1.8 is not
compatible with Angular 14. Apparently,
it's been fixed in a dev release but it's not
stable yet. Have a look here
https://github.com/ionic-team/ionic-framework/issues/25353
you can update @ionic/angular to
version 6.1.9-dev.11654275237.1b595be3
and re-run npm install.
Should work fine for now, if you wanna be on the edge.

==================================

Fixes #2377

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-29 20:21:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2529" class=".btn">#2529</a>
            </td>
            <td>
                <b>
                    docs(readme): fix broken VS-code badge in the readme
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Replaced the Open in VSCode badge to be backed by the shields.io
service which actually works.
2. Removed the codecov badge for now because it does not work
at the moment due to us having broken up the test execution into
smaller CI jobs that are separate from each other.

Fixes #2169

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-29 07:41:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2528" class=".btn">#2528</a>
            </td>
            <td>
                <b>
                    build(codegen): fix OpenAPI TypeError: error.response.data.on is not a function
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Stopped using the openapi-generator-cli package to download the .jar files
and instead went with a direct download approach after having reverse
engineered the HTTP URLs that can be used for fetching the jars from
the maven repository.
2. The above appears to be a good fix because the third party service
that was serving HTTP 504 errors was not the download link but the
version validator link (e.g. a service that can tell us whether a
specific version of the OpenAPI generator jar file exists or not). So,
now that we just download exactly the versions of the .jars that we need
there is no request sent to that other service and the problem therefore
seems to have been solved.
3. We no longer need to delete the openapitools.json file in the root
because it no longer gets created to begin with due to the change from 1
4. At this point it is really hard to tell if this is the last of this
issue with the OpenAPI generator jar files, but one can hope.
5. Attempting to speed up the CI by optimizing the build-dev job:
It is no longer doing bundle name validation nor the custom checks by
default and it also skips linting and codegen entirely which are now done
by separate jobs that can run in parallel. This should also reduce the
load we place on the public utility service that is hosting the .jar files
for the OpenAPI generator because this way the 40+ CI jobs that we have
at the moment won't each download a pair of >20 MB .jar files every time.

Fixes #2525

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-29 01:24:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2527" class=".btn">#2527</a>
            </td>
            <td>
                <b>
                    ci(test-tooling): fix CI job failing due to with wasm-pack
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated the cactus-rust-compiler version to properly build the image and get the required files.

Fixes https://github.com/hyperledger/cacti/issues/2407

Signed-off-by: adrianbatuto <adrian.batuto@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-29 00:55:46 +0000 UTC
    </div>
</div>

