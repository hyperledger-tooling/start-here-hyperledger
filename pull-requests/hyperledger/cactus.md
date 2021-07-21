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
                PR <a href="https://github.com/hyperledger/cactus/pull/1153" class=".btn">#1153</a>
            </td>
            <td>
                <b>
                    Feat 967 complete request handler and endpoints
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
        Created At 2021-07-20 20:07:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1152" class=".btn">#1152</a>
            </td>
            <td>
                <b>
                    docs(examples): increase supply chain image boot responsiveness #780
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">documentation</span>
            </td>
            <td>
                Added logging to all 3 of the test ledger classes that are being used
which are taking up most of the boot time.
Now users can see the setup process as it chugs along step by step and
in general be much more confident while waiting that things are indeed
happening instead of the container just being in a zombie state.

Also added an additional point in the README.md file claryfying that
one needs to have a working installation of docker on their machine.
Decided to not go into any more detail than that because the (linked)
docker for desktop documentation is the best/most robust resrouces
available there is and it would be hard to compete with it if we were
to produce our own installation instructions.

Fixes #780

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 19:56:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1151" class=".btn">#1151</a>
            </td>
            <td>
                <b>
                    fix(connector-corda): fix build broken by operationId rename
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Corda</span><span class="chip">documentation</span>
            </td>
            <td>
                Also: Update the readmes of other packages where the old name of
the operation/endpoint was still being used as well.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-20 18:47:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1147" class=".btn">#1147</a>
            </td>
            <td>
                <b>
                    test: ensure .test.ts ending for test code files #1137
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #1137

Signed-off-by: Tommesha Wiggins <tommesha.wiggins@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-19 20:42:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1145" class=".btn">#1145</a>
            </td>
            <td>
                <b>
                    style: fix openAPI spec linter warning endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1126

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>
_________________________________
Error message shown below: 


> @hyperledger/cactus-plugin-consortium-manual@0.5.0 tsc
> tsc --project ./tsconfig.json

lerna ERR! npm run tsc exited 2 in '@hyperledger/cactus-api-client'
lerna ERR! npm run tsc stdout:

> @hyperledger/cactus-api-client@0.5.0 tsc
> tsc --project ./tsconfig.json

../cactus-plugin-consortium-manual/dist/types/main/typescript/consortium/get-consortium-jws-endpoint-v1.d.ts(5,17): error TS2307: Cannot find module '../../json/openapi.json' or its corresponding type declarations.
../cactus-plugin-consortium-manual/dist/types/main/typescript/consortium/get-node-jws-endpoint-v1.d.ts(5,17): error TS2307: Cannot find module '../../json/openapi.json' or its corresponding type declarations.
lerna ERR! npm run tsc exited 2 in '@hyperledger/cactus-api-client'
lerna WARN complete Waiting for 4 child processes to exit. CTRL-C to exit immediately.
ERROR: "tsc" exited with 2.
ERROR: "build:dev:backend" exited with 1.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 20:30:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1141" class=".btn">#1141</a>
            </td>
            <td>
                <b>
                    build: migrate to Yarn v1 from npm v7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span><span class="chip">dependent</span>
            </td>
            <td>
                ## Dependencies

Depends on #1111 

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: Thu Jul 15 2021 22:10:04 GMT-0700 (Pacific Daylight Time)
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: Thu Jul 15 2021 22:12:29 GMT-0700 (Pacific Daylight Time) 

build: migrate to Yarn v1 from npm v7
    
Why?
It was reported by other maintainers that yarn behaves much
better in corporate proxy/firewalled environments.

Future plans: Once Berry (Yarn v2) is stable, we should take
a look at migrating onto that one. I did give it a try this
time to see if their release candidate happened to be stable
enough but it was not unfortunately (there were dependency
resolution issues that lead the Yarn v2 not installing
certain runtime dependencies at all so v1 it is for now)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-16 05:18:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1139" class=".btn">#1139</a>
            </td>
            <td>
                <b>
                    chore(release): publish v0.6.0
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
        Created At 2021-07-15 23:00:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1136" class=".btn">#1136</a>
            </td>
            <td>
                <b>
                    docs(examples): supply chain- eliminate endpoint constant classes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span>
            </td>
            <td>
                
Fixes #1120

Signed-off-by: Youngone Lee <youngone.lee@accenture.com>

@petermetz ping for review :) 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 19:52:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1135" class=".btn">#1135</a>
            </td>
            <td>
                <b>
                    refactor(core-api): keychain plugin get/set generic type parameters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refactor(core-api): keychain plugin get/set generics #1135 

Fixes #1135 
Signed-off-by: Tommesha Wiggins <tommesha.wiggins@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 18:18:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1134" class=".btn">#1134</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): OpenAPI spec validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                add missing validation from plugin REST endpoints

fixes #847

Signed-off-by: Elena Izaguirre <e.izaguirre.equiza@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 15:52:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1133" class=".btn">#1133</a>
            </td>
            <td>
                <b>
                    feat(connector-fabric): endorsing peers request arg #1122
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">dependent</span><span class="chip">enhancement</span>
            </td>
            <td>
                Makes it possible to set the endorsing peers on a transaction
when submitted through the Fabric connector.

For example these values can be passed in to the new parameter
and it will set the endorsers up accordingly prior to submitting
the transaction to the ledger:
- org1.example.com
- Org1MSP
- org2.example.com
- Org2MSP

(You only need either the org domain or the msp ID, no need
to specify both of them for it to work).

For a working example, see this test case:
packages/cactus-plugin-ledger-connector-fabric/src/test/typescript/integration/fabric-v2-2-x/run-transaction-endpoint-v1.test.ts

Depends on #1123
Depends on #1130

Fixes #1122

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 06:15:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1132" class=".btn">#1132</a>
            </td>
            <td>
                <b>
                    feat(connector-fabric): identity json signing credentials #1130
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">dependent</span><span class="chip">enhancement</span>
            </td>
            <td>
                Introduces a new, optional (for now) parameter on the run tx
endpoint's request object called gatewayOptions which is capable
of including everything that one needs to instantiate a gateway
object of the underlying Fabric Node SDK.

This change makes it possible to not need the keychain plugin
at all when someone does not need/want it.

Fixes #1130

Depends on #1124

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 04:56:31 +0000 UTC
    </div>
</div>

