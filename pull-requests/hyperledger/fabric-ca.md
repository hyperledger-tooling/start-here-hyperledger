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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/337" class=".btn">#337</a>
            </td>
            <td>
                <b>
                    test flake branch - DO NOT MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **DO NOT MERGE**

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 13:22:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/336" class=".btn">#336</a>
            </td>
            <td>
                <b>
                    Build multi-arch docker images with docker buildx - DO NOT MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **DRAFT PR - DO NOT MERGE**

This PR is currently configured to push docker images and release binary archives up to hyperledgendary/fabric-ca and ghcr.io.   This will allow us to test the mechanics of building, publishing, etc. on a repo other than docker.io prior to the 1.5.6 release. 


Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- New feature

#### Description

This PR adds support for multi-arch Docker images, generated with the `buildx` builder.

Release actions are triggered by applying a semrev tag to the repo at the target commit.  With this PR there is no need to manually launch the release pipeline, other than by applying the tag to the target commit / branch.

#### Additional details

The main challenge with this PR was not the addition of the GHA pipeline to run with buildx, but the dependency on `CGO` for the platform-specific compilation of sqlite C code.  When compiling the binaries within the _docker context_, the cross-compiling tool chains are not used, reverting to the stock gcc and letting QEMU sort out the details up at the buildx layer.

One area for additional review is that the alpine images do not have 100% coverage of glibc, and a function referenced by the sqlite engine fell through the cracks.  This PR changes the base / builder from golang-alpine to golang, runs a static link of the sqlite / cgo external routines, and installs `gcompat` in the alpine image along with the fabric binaries.  The resulting Docker images are kept small (~25MB) by distributing a minimal alpine, and seem like they are working well on all the target platforms.

Unfortunately the fabric-ca-fvt images could not be ported over to an arm64 runtime, as there are several dependencies installed to the test image that do not include native support for arm64.   When running the fvt tests, the container can be launched on an amd64 machine or under emulation with QEMU. 

#### Related issues

- https://github.com/hyperledger/fabric/issues/2994#issuecomment-1170102505 



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 02:43:21 +0000 UTC
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

