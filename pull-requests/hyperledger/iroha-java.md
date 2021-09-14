---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/141" class=".btn">#141</a>
            </td>
            <td>
                <b>
                    Altered coroutine scope from Global and renamed some methods 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: rkharisov <rinat@soramitsu.co.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 09:52:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/140" class=".btn">#140</a>
            </td>
            <td>
                <b>
                    Added proper handling of errors can be thrown by client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: rkharisov <rinat@soramitsu.co.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 08:38:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/139" class=".btn">#139</a>
            </td>
            <td>
                <b>
                    Generated model after schema changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: rkharisov <rinat@soramitsu.co.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-14 06:47:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/138" class=".btn">#138</a>
            </td>
            <td>
                <b>
                    Removed PublicKeyWrapper due it shadowed default encoding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently we have wrappers for public and private keys what just override encoding format of the keys derived from third-party library. Library itself encodes them in X.509 format. We do not work with such format, but instead work with raw format. In this PR I made encoding explicit with introducing extension function. So encoding to X-509 is not shadowed buy our implementation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 13:13:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/137" class=".btn">#137</a>
            </td>
            <td>
                <b>
                    Client exception handling, granting mint permission
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                added instruction grantMintUserAssetsDefinition to allow user to mint the asset registered by another user, wrapped ktor iroha client exceptions

Signed-off-by: mbubnov <bubnov@soramitsu.co.jp>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-10 11:11:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/136" class=".btn">#136</a>
            </td>
            <td>
                <b>
                    Add assetsByDomainName query
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * added assetsByDomainName query
* implemented AssetsExtractor for parsing list of assets results
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-08 14:31:22 +0000 UTC
    </div>
</div>

