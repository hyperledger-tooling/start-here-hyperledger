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
                PR <a href="https://github.com/hyperledger/fabric/pull/4678" class=".btn">#4678</a>
            </td>
            <td>
                <b>
                    Switch to bccsp, metrics, flogging in fabric-lib-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following packages are being moved from fabric to fabric-lib-go so that they can be shared across fabric and fabric-ca:

- github.com/hyperledger/fabric/bccsp
- github.com/hyperledger/fabric/common/flogging
- github.com/hyperledger/fabric/common/metrics (including the gendoc utility)

The [PR](https://github.com/hyperledger/fabric-ca/pull/404) over in fabric-ca finally removes the fabric-ca dependency on core fabric.

This commit updates fabric to use the common code in fabric-lib-go.

For now a temporary branch in fabric-lib-go is used, see the corresponding [commit](https://github.com/hyperledger/fabric-lib-go/commit/cdae4d4a292dbad122b93a2c5c70bc61d846e990).
After this PR is reviewed and merged fabric-lib-go will be released and the dependency here will be updated to a real versioned release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 02:52:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4674" class=".btn">#4674</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/tools from v0.14.0 to v0.17.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump golang.org/x/tools to v0.17.0.

Note that gendoc broke with v0.15.0 with error:
panic: can't determine type sizes for compiler "" on GOARCH ""

It turns out that gendoc didn't need the problematic `packages.NeedTypesInfo` and therefore this option is now removed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 20:40:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4673" class=".btn">#4673</a>
            </td>
            <td>
                <b>
                    Block Censorship Test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Test update: Add a test that will checkout how the block deliverer acts with a malicious orderer that censors blocks.

Description: The test creates a network, creates blocks on the chain, replaces the orderers with mocks and communicates with the peer. One of the orderers becomes malicious and after delivering a few data blocks he will stop. Afterwards the peer will ask for another orderer to deliver the data blocks, which should be successful, since he should be a honest orderer.

arkadi.piven@ibm.com

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 13:44:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4672" class=".btn">#4672</a>
            </td>
            <td>
                <b>
                    Bump github.com/IBM/idemix and consensys/gnark-crypto (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump github.com/IBM/idemix to get updated github.com/consensys/gnark-crypto.

Note that github.com/IBM/idemix pulls in github.com/kilic/bls12-381, which requires build tag "generic" to compile on amd64 in plugin mode.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 02:04:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4670" class=".btn">#4670</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd to 1.6.26 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump github.com/containerd/containerd from 1.6.18 to 1.6.26
Only move golang.org/x/tools to v0.14.0 (later versions introduce an issue with ./scripts/metrics_doc.sh check)
Only move google.golang.org/protobuf to v1.31.0 (later versions introduce an issue with chaincode build)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 14:31:19 +0000 UTC
    </div>
</div>

