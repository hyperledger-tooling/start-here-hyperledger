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
                PR <a href="https://github.com/hyperledger/cactus/pull/1111" class=".btn">#1111</a>
            </td>
            <td>
                <b>
                    build(typescript): use project references compiler feature #312
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WORK IN PROGRESS

Fixes #312
Fixes #973

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-07 01:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1110" class=".btn">#1110</a>
            </td>
            <td>
                <b>
                    remove magic strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1104

Signed-off-by: Hana Awad <awadhana0825@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-06 17:32:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1109" class=".btn">#1109</a>
            </td>
            <td>
                <b>
                    feat(keychain-vault): add the missing endpoint classes #676
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Keychain</span><span class="chip">enhancement</span>
            </td>
            <td>
                1. Adds the has/delete endpoints (which were missing completely)
2. Adds the get/set endpoints which were partially already implemented.
3. Moves the express dependency to be a dev dependency since we only
use the types (e.g. only needed at compile time, not at runtime)
4. Adds specific test cases to the API client verifying the
get/set/has/delete endpoints
5. Renames the getKeychainEntry and setKeychainEntry operationIDs
to have a V1 suffix.

Fixes #676

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

cc: @Zzocker @sichen1234
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-03 20:08:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1107" class=".btn">#1107</a>
            </td>
            <td>
                <b>
                    ci(containerization): build all container images via the CI suite #942
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">dependencies</span><span class="chip">dependent</span>
            </td>
            <td>
                This will get us closer to the desired state of affairs where any
source code change that breaks the build can be detected prior
to the pull request getting merged.

Before this, the issue was that DockerHub would not integrate
properly with the GitHub PR Checks mechanism and so we were
unable to have the checks executed properly.

Fixes hyperledger#942

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

Depends on #1105
Depends on #1106
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 03:20:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1106" class=".btn">#1106</a>
            </td>
            <td>
                <b>
                    fix(connector-corda): kotlin compilation error due to missing method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Corda</span><span class="chip">bug</span>
            </td>
            <td>
                When we added the prometheus monitoring endpoint to the
OpenAPI spec, the kotlin implementation was not updated
and this has lead to the container image build process failing
which was not noticed because currently the GHA CI does not
build the container images and therefore you can get away
with introducing issues to the container image build.
(this is soon to be rectified)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 02:56:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/1105" class=".btn">#1105</a>
            </td>
            <td>
                <b>
                    docs(examples): migrate containers to ubuntu-20.04 Docker-in-Docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">documentation</span>
            </td>
            <td>
                This restores the supply chain example app into a working state.

Also migrated the carbon accounting example app onto the new base
image, but that one isn't fully functional just yet (but at least the
contanier build isn't broken anymore which is already signfiicant
progress.)

The image built from this revision of the source code has been
tagged on the container registry as:
ghcr.io/hyperledger/cactus-example-supply-chain-app:2021-07-01--fix-1063-v2

Fixes #1063

(this is the second try to fix that issue, the previous one failed)

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-02 02:17:09 +0000 UTC
    </div>
</div>

