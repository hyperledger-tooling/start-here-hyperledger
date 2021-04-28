---
layout: default
title: fabric-opssc
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-opssc
---

# fabric-opssc <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-opssc){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    chore(*): Support both Fabric v2.3 and v2.2 series
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch makes it possible to support not only Fabric v2.3 series
but also v2.2 series.

To do that, this patch includes:
- Update build scripts to enable to create docker images of OpsSC for
the specified Fabric version
- Update integration tests to enable to run tests using the specified
Fabric version
- Update the related documents

Also, this includes the following minor fixes:
- Fix the docker compose network name for `test-network` with `fabric_test`
- Update npm packages
  - Especially update the version of `fs-extra` to avoid the typescript complie error
- Remove the hard code parts in `/version` API of the API server

Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 06:23:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-opssc/pull/8" class=".btn">#8</a>
            </td>
            <td>
                <b>
                    docs(chaincode): Add design memo for state transition of chaincode_ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Tatsuya Sato <tatsuya.sato.so@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 02:32:10 +0000 UTC
    </div>
</div>

