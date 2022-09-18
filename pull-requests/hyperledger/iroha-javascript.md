---
layout: default
title: iroha-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-javascript
---

# iroha-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/125" class=".btn">#125</a>
            </td>
            <td>
                <b>
                    feat: update lib with latest proto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated the proto files using these [proto](https://github.com/hyperledger/iroha/tree/main/shared_model/schema) files.
To generate the ts proto files I used the following script:
```
PROTOC_GEN_TS_PATH="../../node_modules/.bin/protoc-gen-ts"

OUT_DIR="./"

protoc \
    --plugin="protoc-gen-ts=${PROTOC_GEN_TS_PATH}" \
    --js_out="import_style=commonjs,binary:${OUT_DIR}" \
    --ts_out="${OUT_DIR}" \
    *.proto
```
Signed-off-by: yashrajdesai <yashrajdesai30@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-18 11:42:25 +0000 UTC
    </div>
</div>

