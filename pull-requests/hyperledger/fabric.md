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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4667" class=".btn">#4667</a>
            </td>
            <td>
                <b>
                    Fix bft handle request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description

The `HandleRequest` in `BFTChain` should call `HandleRequest` of consensus (and not `SubmitRequest`).
And the request is already verified inside, so no need to verify here.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-05 09:27:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4666" class=".btn">#4666</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc to 1.1.12 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump github.com/opencontainers/runc to 1.1.12 (release-2.2)
Only move golang.org/x/tools to v0.14.0 (later versions introduce an issue)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 21:47:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4665" class=".btn">#4665</a>
            </td>
            <td>
                <b>
                    Bump github.com/opencontainers/runc to 1.1.12 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump github.com/opencontainers/runc to 1.1.12 (release-2.5)
Only move golang.org/x/tools to v0.14.0 (later versions introduce an issue with ./scripts/metrics_doc.sh check)
Only move google.golang.org/protobuf to v1.31.0 (later versions introduce an issue with chaincode build)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 21:44:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4664" class=".btn">#4664</a>
            </td>
            <td>
                <b>
                    Bump github.com/containerd/containerd from 1.6.18 to 1.6.26
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

Update tests to reflect message updates in latest grpc v1.61.0.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 19:04:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4663" class=".btn">#4663</a>
            </td>
            <td>
                <b>
                    Upgrade github.com/sirupsen/logrus to v1.9.3.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description

Upgrade github.com/sirupsen/logrus from v1.8.1 to v1.9.3.
#### Additional details

Necessary dependency patch. Backport.

#### Related issues

N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 18:45:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4662" class=".btn">#4662</a>
            </td>
            <td>
                <b>
                    Upgrade github.com/sirupsen/logrus to v1.9.3.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Upgrade github.com/sirupsen/logrus from v1.9.0 to v1.9.3.

#### Additional details

Required patch.

#### Related issues

N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 18:42:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4659" class=".btn">#4659</a>
            </td>
            <td>
                <b>
                    Upgrade srupsen/logrus.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description

Upgrade github.com/sirupsen/logrus to v1.9.3.

#### Additional details

Necessary patch.  This is for the `main` branch.

#### Related issues

N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 18:27:48 +0000 UTC
    </div>
</div>

