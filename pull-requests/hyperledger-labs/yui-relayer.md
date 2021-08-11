---
layout: default
title: yui-relayer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/yui-relayer
---

# yui-relayer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/yui-relayer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/47" class=".btn">#47</a>
            </td>
            <td>
                <b>
                    Add corda2fab E2E test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This resolves a part of https://github.com/hyperledger-labs/yui-relayer/issues/26.


In the `corda-build` job, fabric-chaincode docker images are rebuilt and saved.
This is needed to pack `yui-corda-ibc-lightclientd` and `fabibc` in a single docker image.

Along with this, the base image for fabric-chaincode images is changed from `alpine` to `buster`.
`yui-corda-ibc` doesn't compile on `alpine`-based images because of https://github.com/google/protobuf-gradle-plugin/issues/265.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 08:15:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/yui-relayer/pull/46" class=".btn">#46</a>
            </td>
            <td>
                <b>
                    Add Docker image of Ganache node for testing
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
        Created At 2021-08-04 11:50:27 +0000 UTC
    </div>
</div>

