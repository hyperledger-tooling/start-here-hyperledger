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
                PR <a href="https://github.com/hyperledger/fabric/pull/3882" class=".btn">#3882</a>
            </td>
            <td>
                <b>
                    Switch base docker image from golang-alpine to ubuntu:20.04
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

This PR switches the Fabric base docker images from golang-alpine to ubuntu:20.04.  The upgrade is necessary as the golang-alpine libc runtimes (musl) are incompatible with the requirements on multi-arch runtimes. 

The motivations for this upgrade are described in detail in Discussion #3876 and comments in DRAFT PR #3877 


#### Additional details

- Discussion #3876 
- PR #3877  (DRAFT)


#### Related issues

- #2994
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 15:00:25 +0000 UTC
    </div>
</div>

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

