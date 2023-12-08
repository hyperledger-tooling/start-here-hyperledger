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
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    build(deps): migrate from grpc to @grpc/grpc-js and make it a prod dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha1</span>
            </td>
            <td>
                BREAKING CHANGE: When creating a gRPC Iroha service instance such as
`CommandService` or `QueryService` you have to make sure to create the
credentials object that you will use to construct the service instances
from the new gRPC library. Otherwise your code will throw, claiming that
you have not passed in a valid credentials object (even though you did,
just with the wrong version of the gRPC library)

Primary changes:
===============

1. Migrate over from the legacy and unmaintained grpc to @grpc/grpc-js
2. Move from `devDependencies` to `dependencies` so that is a production
dependency of the package.

Secondary changes:
==================

1. Ignored the .yarn/cache directory in git so that there aren't 400
new files in the git index after a `yarn install` execution on the terminal.

Fixes https://github.com/hyperledger/iroha-javascript/issues/173

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-02 06:22:29 +0000 UTC
    </div>
</div>

