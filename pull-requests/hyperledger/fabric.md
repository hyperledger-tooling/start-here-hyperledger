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
                PR <a href="https://github.com/hyperledger/fabric/pull/3874" class=".btn">#3874</a>
            </td>
            <td>
                <b>
                    Updates to Pygments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-18 08:53:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3872" class=".btn">#3872</a>
            </td>
            <td>
                <b>
                    Run a full external link for CGO against musl when building in Docker
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

This PR runs a full static link, at compile-time, for CGO against libmusl when building docker images.  This is required for proper support of PKCS11 / HSM libraries, which require CGO.

#### Related issues

- Issue #3867 
- Issue #3372 (tangentially)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 14:06:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3871" class=".btn">#3871</a>
            </td>
            <td>
                <b>
                    Scheduled vulnerability scan of dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes to #3860
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 10:55:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3870" class=".btn">#3870</a>
            </td>
            <td>
                <b>
                    Security vulnerability scanning using govulncheck (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a makefile target for vulnerability scanning, which can later be used for scheduled vulnerability scans.

Cherry-pick of e6808b162f889a0b568e98731d39cf64afcb79b0 from main branch.

Contributes to https://github.com/hyperledger/fabric/issues/3860
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 10:49:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3869" class=".btn">#3869</a>
            </td>
            <td>
                <b>
                    Security vulnerability scanning using govulncheck (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a makefile target for vulnerability scanning, which can later be used for scheduled vulnerability scans.

Cherry-pick of e6808b162f889a0b568e98731d39cf64afcb79b0 from main branch.

Contributes to #3860
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 10:48:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3868" class=".btn">#3868</a>
            </td>
            <td>
                <b>
                    Security vulnerability scanning using govulncheck (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a makefile target for vulnerability scanning, which can later be used for scheduled vulnerability scans.

Cherry-pick of e6808b162f889a0b568e98731d39cf64afcb79b0 from main branch.

Contributes to #3860
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-16 10:48:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3866" class=".btn">#3866</a>
            </td>
            <td>
                <b>
                    Conditionally publish docker images to docker.io (backport #3865)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3865 done by [Mergify](https://mergify.com).


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
        Created At 2022-12-15 20:00:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3865" class=".btn">#3865</a>
            </td>
            <td>
                <b>
                    Conditionally publish docker images to docker.io
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- CI pipeline 

#### Description

This PR changes the release-2.5 branch container registry target from ghcr.io to docker.io.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 18:48:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3863" class=".btn">#3863</a>
            </td>
            <td>
                <b>
                    change order of raft state change notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description
Change the order of notification about the raft state change,
first to chain loop and then abdicateleadership go rountine.

#### Additional details
Analysis and observation noted down in the issue: https://github.com/hyperledger/fabric/issues/3629#issuecomment-1353191438 

#### Related issues
#3629 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 15:09:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3862" class=".btn">#3862</a>
            </td>
            <td>
                <b>
                    Address several SIGSEGV errors encountered in fabric-test with alpha1 (backport #3861)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3861 done by [Mergify](https://mergify.com).


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
        Created At 2022-12-15 14:35:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3861" class=".btn">#3861</a>
            </td>
            <td>
                <b>
                    Address several SIGSEGV errors encountered in fabric-test with alpha1
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

This removes the external static link option from release builds


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 13:19:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3859" class=".btn">#3859</a>
            </td>
            <td>
                <b>
                    Security vulnerability scanning using govulncheck
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a makefile target for vulnerability scanning, which can later be used for scheduled vulnerability scans.

Contributes to #3860
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-15 11:38:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3857" class=".btn">#3857</a>
            </td>
            <td>
                <b>
                    Prepare static binaries for release targets and docker runtimes, and dynamic binaries for local dev
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

This PR fixes two problems with the release-2.5 Makefile: 

- On rancher desktop, `TARGETOS` AND `TARGETARCH` are not automatically set by the "docker" build agent, leading to an error when building the image locally without `buildx` or builders from docker.io.   This sets the variables to `linux` and `go env GOARCH` when building the containers locally, aligning with the default values set by buildx.

- The introduction of statically linked binaries was necessary for running ARM64 on the Alpine containers, but it caused a regression and forced the peer to sigsegv when built _locally_ on an emulated ubuntu64 linux.   With this update, the locally built peer images will continue to be created as dynamically linked binaries, with the static linking enabled only for the release target and for binaries deployed to alpine in Docker. 

#### Related issues

- #2994 
- #3372 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 20:22:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3856" class=".btn">#3856</a>
            </td>
            <td>
                <b>
                    Prepare static binaries for release targets and docker runtimes, and dynamic binaries for local development
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Bug fix

#### Description

This PR fixes two problems with the release-2.5 Makefile: 

- On rancher desktop, `TARGETOS` AND `TARGETARCH` are not automatically set by the "docker" build agent, leading to an error when building the image locally without `buildx` or builders from docker.io.   This sets the variables to `linux` and `go env GOARCH` when building the containers locally, aligning with the default values set by buildx.

- The introduction of statically linked binaries was necessary for running ARM64 on the Alpine containers, but it caused a regression and forced the peer to sigsegv when built _locally_ on an emulated ubuntu64 linux.   With this update, the locally built peer images will continue to be created as dynamically linked binaries, with the static linking enabled only for the release target and for binaries deployed to alpine in Docker. 

#### Related issues

- #2994 
- #3372 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 20:02:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3855" class=".btn">#3855</a>
            </td>
            <td>
                <b>
                    Update command docs - remove unnecessary orderer flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The CLI commands "querycommitted" and "checkcommitreadiness" only query a peer, they do not interact with an orderer node. Therefore the orderer flags -o --tls --cafile are not needed on these commands.

Update the command reference docs and user docs accordingly.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 19:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3854" class=".btn">#3854</a>
            </td>
            <td>
                <b>
                    Reconciliation changes for purged private data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- New feature

#### Description
This PR changes the reconciliation code for taking private data purge into consideration

#### Related issues
Closes #3027 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 14:38:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3853" class=".btn">#3853</a>
            </td>
            <td>
                <b>
                    Remove duplicate ThreeOrgRaft nwo network
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A duplicate ThreeOrgEtcdRaft was introduced in #3643 so removing the original network

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-14 12:39:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3851" class=".btn">#3851</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.9 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.9

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 20:16:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3850" class=".btn">#3850</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.18.9

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-13 20:12:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3849" class=".btn">#3849</a>
            </td>
            <td>
                <b>
                    Update purge private data integration tests (backport #3819)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3819 done by [Mergify](https://mergify.com).


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
        Created At 2022-12-13 19:48:25 +0000 UTC
    </div>
</div>

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

