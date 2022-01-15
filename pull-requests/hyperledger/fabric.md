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
                PR <a href="https://github.com/hyperledger/fabric/pull/3174" class=".btn">#3174</a>
            </td>
            <td>
                <b>
                    replace arm64 with amd64 for installation scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Rohan Shrothrium <shrothriumrohan@gmail.com>

While using the new mac books which has an arm64 infrastructure, the installation and bootstrap script fails as there is no specific binaries for arm64. I downloaded the amd64 binaries and fabric images and they work as expected on the new M1 architecture.

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
This PR incorporates changes to download the amd64 binaries and images for an arm64 architecture.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 09:22:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3173" class=".btn">#3173</a>
            </td>
            <td>
                <b>
                    Update chaincode4ade.rst
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                typo in 'oreder'

#### Type of change
- Documentation update

#### Description
There was a typo in the word 'oreder'. Changed it to 'order'
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-15 07:38:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3172" class=".btn">#3172</a>
            </td>
            <td>
                <b>
                    Close connections to stale ordering nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes grpc connections to ordering nodes when they are no longer part of any channel configuration.

Resolves https://github.com/hyperledger/fabric-gateway/issues/345

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 13:52:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3171" class=".btn">#3171</a>
            </td>
            <td>
                <b>
                    Refactor gateway Endorse() method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To improve readability and ease of maintenance

Resolves #3122 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 13:50:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3167" class=".btn">#3167</a>
            </td>
            <td>
                <b>
                    Maintain Pvt data hashed index
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds code for creating hashed index entries during block commit and deleting the hashed index entries during purge triggered by _Block to live_ based expiry

#### Type of change
- New feature

#### Additional details
The indexes needs also to be maintained when the private data is committed via reconciliation. However, this will be covered in a separate story (issue #3027) because, during reconciliation we need to take care of trimming the already purged data, if any.

#### Related issues
issue #3023 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 05:25:17 +0000 UTC
    </div>
</div>

