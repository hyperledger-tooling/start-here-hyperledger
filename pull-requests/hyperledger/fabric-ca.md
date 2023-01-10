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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/347" class=".btn">#347</a>
            </td>
            <td>
                <b>
                    Fix the interop-test build
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

In PR #346, the CA base docker image was switched from alpine-golang to ubuntu.  In the new image, golang is now installed with curl using the `GO_VER`, `TARGETOS`, AND `TARGETARCH` build args.

Depending on the version of Docker installed on the build host, `TARGETOS` and `TARGETARCH` are not always available in the build context.  (In recent Docker versions, these args are implicit in the build context.)  For instance, the fabric-interop tests at Azure are currently failing when trying to build a CA docker image. 

This PR passes the target arch/os from the Makefile to docker as build args.

#### Related issues

- Example [interop test failure](https://dev.azure.com/Hyperledger/Fabric-Test/_build/results?buildId=59844&view=logs&j=a183ae4c-f3a4-5b00-aa7e-db0d3d65a8b9&t=80753e5a-ca3e-565c-aa73-31a966f12831) at azure. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 13:14:44 +0000 UTC
    </div>
</div>

