---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3847" class=".btn">#3847</a>
            </td>
            <td>
                <b>
                    Publish multi-arch docker images and binaries for arm64, amd64
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

Builds multi-arch Docker images and native binaries for arm64 and amd64.

#### Additional details

This PR is a "cherry-pick" (back/forward) port of the following PRs from the release-2.5 branch "up" into the mainline: 

- PR #3843 
- PR #3839 
- PR #3837 
- PR #3836 


#### Related issues

- #2994 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 18:44:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3846" class=".btn">#3846</a>
            </td>
            <td>
                <b>
                    Support linux-arm64 with install-fabric.sh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Bug fix

#### Description

When installing fabric CLI, the install-fabric.sh was overriding the platform arch incorrectly when installing on arm64 chipsets.

On linux, it was reading from `aarch64` 
On darwin, it was reading from `amd64`

Installer now downloads binaries from `${PLATFORM}`, defined as `${OS}-${ARCH}`, using the equivalent tokens as `go env GOOS` or `go env GOARCH` 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 14:46:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3845" class=".btn">#3845</a>
            </td>
            <td>
                <b>
                    Add purge private data documentation (backport #3841)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3841 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-09 17:45:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3843" class=".btn">#3843</a>
            </td>
            <td>
                <b>
                    Publish release artifacts to conventional installation paths
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Bug fix

#### Description

This PR updates the release pipeline to publish binary assets to the traditional paths within the GH Release.

In addition, this applies the `TWO_DIGIT_VERSION` release tag, without the leading 'v', to determine the coordinates of the embedded ccenv builder image.

This PR updates the target version of `install-fabric.sh` to 2.5.0 / 1.5.6, and includes an optional `FABRIC_DOCKER_REGISTRY` environment variable in order to override the default Docker Hub container registry.


#### Related issues

#### Release Note

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 21:27:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3842" class=".btn">#3842</a>
            </td>
            <td>
                <b>
                    Update purge private data integration tests (backport #3838)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3838 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 20:49:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3841" class=".btn">#3841</a>
            </td>
            <td>
                <b>
                    Add purge private data documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add docs for the v2.5 purge private data functionality.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 12:15:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3839" class=".btn">#3839</a>
            </td>
            <td>
                <b>
                    fix the multi-arch Docker peer build again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Bug fix
- New feature

#### Description

This PR runs the Fabric release pipeline correctly as a "release" practice triggered through GH.

The `FABRIC_VER` of a component is inferred from the _semrev_ tag applied by the Release process.   The `FABRIC_VER` is applied throughout the Makefile, docker images, and metadata encoded into the client binaries.


#### Additional details

This commit: 

- Adds a work-around for concurrency issues encountered when building multiple target architectures with buildx in parallel.  When multiple buildx builders run concurrently, an unpredictable but frequent error occurs when communicating with the buildx builder.  This manifests as "Error : 403 Forbidden" when pushing _some but not all_ of the image layers to ghcr.io.   This is most likely a resource (CPU, disk, RAM, etc.) being exhausted on the GH executor, and NOT an authentication error when connecting to the container registry.    (Serializing the buildx builder steps seems to have eliminated the sporadic crash.) 

- Solves a `SIGSEGV` error encountered when running the dynamically linked (peer, orderer, etc.) images on the alpine arm64 images.  The problem stems from producing a dynamically linked (libc.so) executable on the golang-alpine base image, copying it, and running on a vanilla alpine container.   (Alpine does NOT include support for libc, and something is either wrong with the libmusl for arm64, or it worked by accident on the amd64.)

```
$(BUILD_DIR)/bin/%: GO_LDFLAGS += -w -extldflags '-static'
```

#### Related issues

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 19:06:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3838" class=".btn">#3838</a>
            </td>
            <td>
                <b>
                    Update purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test purge private data handles state based endorsement correctly

Signed-off-by: James Taylor <jamest@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 17:19:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3837" class=".btn">#3837</a>
            </td>
            <td>
                <b>
                    fix the multi-arch Docker peer build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 21:25:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3836" class=".btn">#3836</a>
            </td>
            <td>
                <b>
                    Build release binaries and Docker images for arm64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR publishes multi-arch Docker images to ghcr.io and prepares native CLI binaries as part of the release process.

(Note:  for the 2.5 release line, the `DOCKER_REGISTRY` attribute in release.yaml will need to be updated to refer to docker.io.  The use of the ghcr.io container registry allows us to run through a few test pipelines and recover from errors without pulling in the HL team to manually scrub artifacts.)

To trigger the release action, draft a new GH Release, applying a semrev tag (e.g. v2.5.0-alpha) to a target branch.  When GH applies the release tag, this will trigger the new release pipeline, generating docker images and fabric CLI binaries.

Signed-off-by: Josh Kneubuhl [jkneubuh@us.ibm.com](mailto:jkneubuh@us.ibm.com)


#### Type of change

- New feature

#### Description

This PR adds support for multi-arch Docker images, generated with the buildx builder.

This PR also modifies the fabric native binaries to include the {{ github.ref_name }} directly when compiling the routine metadata. This allows for a semantic revision (e.g. v2.5.0, v2.5.0-alpha, etc.) or branch relative tags to be associated with the images and binaries. 


#### Additional details


#### Related issues

- Issue #2994 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 18:05:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3834" class=".btn">#3834</a>
            </td>
            <td>
                <b>
                    remove old information from whatis page (backport #3833)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3833 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 14:14:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3833" class=".btn">#3833</a>
            </td>
            <td>
                <b>
                    remove old information from whatis page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>

#### Type of change

- Documentation update

#### Description

remove old information from whatis page

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 14:09:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3832" class=".btn">#3832</a>
            </td>
            <td>
                <b>
                    set Orderer SendBufferSize to 100 as default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                10 has shown to be a bottleneck for Raft performance. 100 appears to be a better default, so proposing that this value is set to 100 by default

Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>

#### Type of change

- Improvement (improvement to code, performance, etc)


#### Description

10 has shown to be a bottleneck for Raft performance. 100 appears to be a better default, so proposing that this value is set to 100 by default


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 12:08:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3831" class=".btn">#3831</a>
            </td>
            <td>
                <b>
                    set Orderer SendBufferSize to 100 as default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                10 has shown to be a bottleneck for Raft performance. 100 appears to be a better default, so proposing that this value is set to 100 by default

Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

10 has shown to be a bottleneck for Raft performance. 100 appears to be a better default, so proposing that this value is set to 100 by default


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-06 10:58:40 +0000 UTC
    </div>
</div>

