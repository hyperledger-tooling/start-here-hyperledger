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
                PR <a href="https://github.com/hyperledger/cacti/pull/2602" class=".btn">#2602</a>
            </td>
            <td>
                <b>
                    fix: use common package convention
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - change package.json and tsconfig.json files to follow common convention

Closes: #2216
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-11 09:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2599" class=".btn">#2599</a>
            </td>
            <td>
                <b>
                    test(connector-fabric): fix tests - package io/fs is not in GOROOT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The simple answer was to upgrade to go v1.20.x from v1.15.x, but this caused a series of other problems that also needed to address so the complete list of changes and their motivations are below:

1. The upgrade to go v1.20.6 1.1. We no longer install docker-compose via pip because since v2 it ships with the main docker package itself (they rewrote it in go) 1.2. Added a new "gcompat" apk package which is necessary because of go v1.20.6 as well. Details on this can be found here: https://github.com/golang/go/issues/59305#issuecomment-1488478737 1.3. As  part of installing the OpenSSH server, we now must first wipe all openssh* packages due to newly surfaced package version conflicts due to the ones that are prepackaged with the alpine image. Without the purge step it fails like this:

       => ERROR [17/64] RUN apk add --no-cache openssh augeas                   1.1s
       ------
       > [17/64] RUN apk add --no-cache openssh augeas:
       0.300 fetch https://dl-cdn.alpinelinux.org/alpine/v3.18/main/x86_64/APKINDEX.tar.gz
       0.560 fetch https://dl-cdn.alpinelinux.org/alpine/v3.18/community/x86_64/APKINDEX.tar.gz
       1.041 ERROR: unable to select packages:
       1.043   openssh-client-common-9.3_p1-r3:
       1.043     breaks: openssh-client-default-9.3_p2-r0[openssh-client-common=9.3_p2-r0]
3. Upgraded the node-ssh library to v13 because v12 was broken due to
changes introduced by the new OpenSSH server.
4. Modified the container image definition so that we have the ability
to customize the version of fabric-nodeenv images used internally by the
peers of the fabric-samples repository. This was needed so that we can
control what version of npm and NodeJS are being used when the chain code
installation process is happening (which is just the peer running the
`npm install --production` command within the fabric-nodeenv container)
5. The default Fabric version used by the testing infrastructure is now
Fabric v2.2.13 and for the NodeJS chain code it is 2.4.2
6. Slightly rearranged the imports & constants in some of the tests
which made it easier to verify that the new image is working as intended.

Fixes #2358
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-08 22:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2598" class=".btn">#2598</a>
            </td>
            <td>
                <b>
                    fix(indy-validator): fix package dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update indy validator python dependencies.
- Add README chapter on updating python dependencies to simplify this process in the future.
- Use pinend ubuntu base image in indy-sdk-cli dockerfile.
- Do some minor README improvements and cleanups.

Tested with `discounted-asset-trade` (should work without an issue now, at least dockerless one)

Depends on: #2596

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-07 09:36:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2597" class=".btn">#2597</a>
            </td>
            <td>
                <b>
                    test(jest): reduce Jest log verbosity - make logs more compact
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Configure jest to override it's internal console logger with the
regular console object provided by the JS runtime.
This way it does not have the extra information printed that is
not useful for 99% of our use-cases (100% of the known ones).

Fixes #2595

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-05 19:44:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2596" class=".btn">#2596</a>
            </td>
            <td>
                <b>
                    build(docker-compose): upgrade to docker compose V2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - `quorum-multi-party-all-in-one`: use newest `quorum-quorum-dev-quickstart`, update quorum versions to most recent available. Run ledger as `quorum` user (required by newer versions). Use docker compose V2 from alpine package registry instead of V1 from pip.
- `besu-multi-party-all-in-one`: similar changes as for quorum-multi-party-all-in-on. Fix broken besu private transaction tests.
- `fabric-all-in-one`: Use docker compose V2 from alpine package registry instead of V1 from pip.
- `sawtooth-all-in-one`: Use docker compose V2 from alpine package registry instead of V1 from pip.

Closes: #2593
Closes: #2557
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-04 17:50:42 +0000 UTC
    </div>
</div>

