---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/338" class=".btn">#338</a>
            </td>
            <td>
                <b>
                     Build multi-arch docker images with buildx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is configured to publish docker images to ghcr.io/hyperledger/fabric-ca. 

This will allow us to test the mechanics of building, publishing, etc. on a repo other than docker.io prior to the formal 1.5.6 release.

To trigger a release action, apply a semrev tag (e.g. `v1.5.6`) to the release target commit. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- New feature


#### Description

This PR adds support for multi-arch Docker images, generated with the buildx builder.
Release actions are triggered by applying a semrev tag to the repo at the target commit.

This PR also modifies the CA binaries to include the `{{ github.ref_name }}` directly when compiling the routine metadata.  This allows for a semantic revision (e.g. `v1.2.3`) strings to be specified as valid version identifiers for the binaries. 

#### Additional details

The main challenge with this PR was not the addition of the GHA pipeline to run with buildx, but the dependency on CGO for the platform-specific compilation of sqlite C code.  What unlocked this feature was to break up the "build" into two separate routes: 

- for client binaries, generate a CGO=1 compiled binary, using a GCC cross-compiler to target a specific architecture.
- for Docker images, use Docker `buildx` to emulate an architecture with QEMU, building with sqlite with GCC.

Unfortunately the fabric-ca-fvt images could not be ported over to an arm64 runtime, as there are several dependencies installed to the test image that do not include native support for arm64. When running the fvt tests, the container can be launched on an amd64 machine or under emulation with QEMU.

I tried to clean up the Makefile with this PR, but triggered a never-ending snowball effect that ended up wedging the FVT tests beyond repair.  There may be some lingering dependencies between unit test outputs that have been mounted accidentally and used as inputs to the FVT container volume mounts.

There may still be some lingering rough edges around statically linking the sqlite objects into golang with glibc, which is not technically supported on alpine.

#### Related issues

* [Native Support For 64bit ARM in fabric fabric#2994 (comment)](https://github.com/hyperledger/fabric/issues/2994#issuecomment-1170102505)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 20:51:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    Remove Azure Pipeline artifacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                With the addition of Github Actions, the old Azure Pipeline CI artifacts can now be removed.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 16:10:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    Fix the build : renew expired test TLS certificates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes the build: 

This PR renews a couple of integration test suite certificates, which had expired.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-30 02:05:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    Build release packages for arm64 CLI binaries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- New feature

#### Description

- Generates arm64 CLI binaries for linux and darwin.

#### Additional details

This PR compiles sqlite3 using CGO on the various platforms.  

#### Related issues

- https://github.com/hyperledger/fabric/issues/2994


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-29 20:40:32 +0000 UTC
    </div>
</div>

