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
                PR <a href="https://github.com/hyperledger/fabric/pull/3879" class=".btn">#3879</a>
            </td>
            <td>
                <b>
                    Trim the (optional) semrev leading 'v' when resolving the ccenv image URL
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

As reported in a [discord thread](https://discord.com/channels/905194001349627914/941396957635682314/1052993323612246097), the semrev 'v' in the peer metadata label is causing the hyperledger/fabric-ccenv:$(TWO_DIGIT_REVISION) label to crash when installing a chaincode package.  This PR strips the (optional) semrev leading `v` character from the two digit rev prior to resolving the chaincode image URL. 

When installing chaincode without this patch, the peer log reports: 
```
2022-12-20 07:54:55.098 EST 0415 DEBU [chaincode.platform] GenerateDockerfile -> 
FROM hyperledger/fabric-baseos:v2.5
ADD binpackage.tar /usr/local/bin
LABEL org.hyperledger.fabric.chaincode.type="GOLANG" \
      org.hyperledger.fabric.version="v2.5.0-alpha3"
ENV CORE_CHAINCODE_BUILDLEVEL=v2.5.0-alpha3
```
... 
```
2022-12-20 07:55:07.111 EST 0418 ERRO [dockercontroller] buildImage -> Error building image: manifest for hyperledger/fabric-baseos:v2.5 not found: manifest unknown: manifest unknown
2022-12-20 07:55:07.111 EST 0419 ERRO [dockercontroller] buildImage -> Build Output:
********************
Step 1/4 : FROM hyperledger/fabric-baseos:v2.5
```


cc: @lehors 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-20 13:41:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3877" class=".btn">#3877</a>
            </td>
            <td>
                <b>
                    COPY static release build artifacts into alpine Docker - DO NOT MERGE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **DO NOT MERGE**

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- New feature

#### Description

This PR resolves the many permutations of SIGSEGV encountered when running multi-arch Fabric 2.5 binaries in Docker.


#### Additional details

There have been several, unsuccessful efforts to unwind the dependencies between multi-stage Docker builds, alpine libc, pkcs11, and CGO native binaries for Fabric.  This has recently appeared as a critical issue for users of Fabric running on an M1 / arm64 system, where the docker based builds regularly SIGSEGV due to the link of golang-alpine's libc/libmusl into the binaries.

This PR resolves the cross-platform issues by *moving the Fabric binary build out of Docker*, relying on golang's multi-arch support to prepare statically linked binaries in an upstream step of the build.  With this simplified model, the reference / release binaries are simply `COPY` steps, removing any and all dependencies on alpine's mangled support for libc.

- Discussion #3876


#### Related issues

- Issue #3837 
- Issue #3867 
- [FAB-2883](https://jira.hyperledger.org/browse/FAB-2883)
- [FAB-3196](https://jira.hyperledger.org/browse/FAB-3196)
- [FAB-18176](https://jira.hyperledger.org/browse/FAB-18176)
- [FAB-16618](https://jira.hyperledger.org/browse/FAB-16618)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 16:50:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3875" class=".btn">#3875</a>
            </td>
            <td>
                <b>
                    Consider purged private data during reconciliation
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

#### Additional details
Cherry-pick (https://github.com/hyperledger/fabric/pull/3854)

#### Related issues
Closes #3027
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 16:18:20 +0000 UTC
    </div>
</div>

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

