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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    Add some debug information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The cert file *must be* `cert.pem`; which in my case it wasn't.  Would have been nice to have some flexibility, however the error messages appeared to be suggestion idemix was an issue, and gave little clue as to what was wrong. 

- update the error message to give more indication of the file that should be checked
- Prevented idemix error from hiding x509

Signed-off-by: Matthew B White <whitemat@uk.ibm.com>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-03 09:06:09 +0000 UTC
    </div>
</div>

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

To trigger the release action, draft a new GH Release, applying a semrev tag (e.g. `v1.5.6-beta`) to a target branch. 

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- New feature


#### Description

This PR adds support for multi-arch Docker images, generated with the buildx builder.

This PR also modifies the CA binaries to include the `{{ github.ref_name }}` directly when compiling the routine metadata.  This allows for a semantic revision (e.g. `v1.2.3`, `v1.2.3-alpha`, etc.) strings to be specified as valid version identifiers for the binaries. 

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

