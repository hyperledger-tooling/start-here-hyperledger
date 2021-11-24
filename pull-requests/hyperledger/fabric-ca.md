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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/267" class=".btn">#267</a>
            </td>
            <td>
                <b>
                    fix expired root.pem certificate - was breaking 8-10 unit test cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

Fixes the following test flakes, caused by a set of expired test certificates: 
```
--- FAIL: TestGetCACert (0.02s)
--- FAIL: TestClientCommandsUsingConfigFile (1.11s)
--- FAIL: TestClientCommandsTLSEnvVar (1.18s)
--- FAIL: TestClientCommandsTLS (1.18s)
FAIL
FAIL	github.com/hyperledger/fabric-ca/cmd/fabric-ca-client/command	36.619s
--- FAIL: TestCWBTLSClientAuth (0.17s)
--- FAIL: TestSRVIntermediateServerWithTLS (2.14s)
--- FAIL: TestSRVRunningTLSServer (1.12s)
--- FAIL: TestSRVTLSAuthClient (3.21s)
--- FAIL: TestPrometheusMetricsE2E (1.23s)
FAIL
FAIL	github.com/hyperledger/fabric-ca/lib	109.721s
FAIL
```

#### Type of change

- Test update

#### Description

Fixes a series of broken fabric-ca unit tests.  These were caused by an expired testdata/root.pem certificate and associated keys.

#### Additional details

`TestCWBTLSClientAuth` is running into some issues when executing with golang 1.17.1.  It is passing OK on the Azure build. 


#### Related issues

Fixes #260 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 21:13:22 +0000 UTC
    </div>
</div>

