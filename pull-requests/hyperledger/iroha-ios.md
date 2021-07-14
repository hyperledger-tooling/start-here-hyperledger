---
layout: default
title: iroha-ios
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-ios
---

# iroha-ios <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-ios){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-ios/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Initial Iroha2 Swift library with schema builder and generated code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Removed Iroha v1 code
Added IrohaSwiftSchemaBuilder project which builds Swift files from Iroha v2 JSON schema
Added IrohaSwiftScale project which contains types required by SCALE, and implementation for Swift Coding to Encode/Decode SCALE types, available as separate Pod
Storing pre-generated schema from latest Iroha v2 schema export
Added utility scripts to generate schema, inject into dev pod or .xcodeproj

Signed-off-by: Alex Oakley <oakley@soramitsu.co.jp>
Closes #128 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 16:04:43 +0000 UTC
    </div>
</div>

