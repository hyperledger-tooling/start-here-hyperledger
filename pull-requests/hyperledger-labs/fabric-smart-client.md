---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    update weaver dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 14:35:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/366" class=".btn">#366</a>
            </td>
            <td>
                <b>
                    Upgrade to ginkgo v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">testing</span>
            </td>
            <td>
                This PR upgrades to ginkgo v2 and enables new functionality such as flaky test retry.

In order to overcome an upgrade conflict where we had v1 and v2 in use, this PR also replaces our impl of ordered and parallel runners with the implementations provided by ifrit. While this replacement does solves the conflict, it also reduces our code base.

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 14:14:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/364" class=".btn">#364</a>
            </td>
            <td>
                <b>
                    Make ATSA Chaincode receipt struct fields public
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue https://github.com/hyperledger-labs/fabric-smart-client/issues/50, removed warnings related to:

SA9005: missing marshaling mechanism

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 12:53:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    Reduce staticcheck warnings (U1000)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As part of issue #50, removed warnings related to:
* U1000: unused variables and functions

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 14:52:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/357" class=".btn">#357</a>
            </td>
            <td>
                <b>
                    Cleanup integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - add integration test generated artifacts to gitignore
- let weaver cleanup testdata folder if test succeeds

Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 10:21:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/356" class=".btn">#356</a>
            </td>
            <td>
                <b>
                    Adding .gitignore to samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Marcus Brandenburger <bur@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-05 09:50:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/355" class=".btn">#355</a>
            </td>
            <td>
                <b>
                    FSC memory enhancements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses the issue of increasing memory consumption as reported in #316.

- Improve integration test runner
The current implementation of runners use goexec to run processes (i.e., orderers, peers, fsc nodes) during our integration tests. goexec uses unbounded buffers to capture the process outputs. While this works nicely for short-living integration tests, other uses of our integration test suite, such as the IOU sample, may ran for long time and will suffer from high memory consumption over the time. Replaces `goexec.Start` with native `cmd.Run` and avoids the use of unbounded buffers. In order to detect when a processes has reached the ready state, we will use a closeable buffer to collect process logs and close it if not needed anymore.

- Replace KVS cache and thereby resolves #339.
The current implementation of our KVS uses an unbounded cache. This cache is replaced with our secondchance cache.

- Vault txidstore is loaded now from config; if not available default cache size is used. default cache size has been reduced to a sane value
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 20:44:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/353" class=".btn">#353</a>
            </td>
            <td>
                <b>
                    committer improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                if a transaction is unknown and is marked as valid by the backend, then there is no need to discard anything from the vault

https://github.com/hyperledger-labs/fabric-token-sdk/pull/335 depends on this PR.

Signed-off-by: Angelo De Caro <adc@zurich.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-04 12:09:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/352" class=".btn">#352</a>
            </td>
            <td>
                <b>
                    Remove cleaning of non-generated file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The main.go under
/integration/fsc/pingpong/cmd/responder
is not generated automatically, hence it should not be cleaned when make clean is invoked

Signed-off-by: Alexandros Filios <alexandros.filios@ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-03 10:17:55 +0000 UTC
    </div>
</div>

