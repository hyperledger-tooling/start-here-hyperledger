---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2206" class=".btn">#2206</a>
            </td>
            <td>
                <b>
                    Add Gary Schulte as Maintainer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Gary has provided [significant commits](https://github.com/hyperledger/besu/commits?author=garyschulte) that have improved the quality of Besu.

Voting ends 2 weeks from the publication of this PR.

For more information on this process see the Becoming a Maintainer section in the MAINTAINERS.md file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 14:54:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2205" class=".btn">#2205</a>
            </td>
            <td>
                <b>
                    Reset updater in case of invalid block : bonsai trie
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

In bonsai trie when we fail to import a block we remain stuck until we restart Besu. I made sure to reset the updater correctly in case of failure to be able to download the new valid block without needing to restart besu.

It happened on the mainnet we received a bad block that failed and then when we received the right block but the node was not able to synchronize

>{"timestamp":"2021-04-28T18:54:15,026","level":"WARN","thread":"EthScheduler-Workers-3","class":"BlockPropagationManager","message":"Failed to import announced block 12330686 (0xfcf34e5f4e403c24c1b70eb1a46c3bda99d45b10fa3d261f2ebf0d2c20867423).","throwable":""}
{"timestamp":"2021-04-28T18:54:15,344","level":"INFO","thread":"EthScheduler-Workers-2","class":"AbstractBlockProcessor","message":"Block processing error: transaction invalid 'NONCE_TOO_LOW'. Block 0xfcf34e5f4e403c24c1b70eb1a46c3bda99d45b10fa3d261f2ebf0d2c20867423 Transaction 0xc834252f73a4f0157fc41924080a9bf2782fd1e0f740cdd1b3011a15db51def1","throwable":""}
{"timestamp":"2021-04-28T18:54:15,353","level":"WARN","thread":"EthScheduler-Workers-2","class":"BlockPropagationManager","message":"Failed to import announced block 12330686 (0xfcf34e5f4e403c24c1b70eb1a46c3bda99d45b10fa3d261f2ebf0d2c20867423).","throwable":""}
{"timestamp":"2021-04-28T18:54:22,469","level":"INFO","thread":"EthScheduler-Workers-0","class":"AbstractBlockProcessor","message":"Block processing error: transaction invalid 'NONCE_TOO_LOW'. Block 0x61d53ccec97be310432f4c333254c143860fed70249b2cd8c8417b19993a8958 Transaction 0x1cef0c4257a8dbb244b54c3de73a0997fcb611a3afd342590c32baf2f73545ce","throwable":""}
{"timestamp":"2021-04-28T18:54:22,469","level":"WARN","thread":"EthScheduler-Workers-0","class":"BlockPropagationManager","message":"Failed to import announced block 12330686 (0x61d53ccec97be310432f4c333254c143860fed70249b2cd8c8417b19993a8958).","throwable":""}
{"timestamp":"2021-04-28T18:54:22,729","level":"INFO","thread":"EthScheduler-Workers-3","class":"AbstractBlockProcessor","message":"Block processing error: transaction invalid 'NONCE_TOO_LOW'. Block 0x61d53ccec97be310432f4c333254c143860fed70249b2cd8c8417b19993a8958 Transaction 0x1cef0c4257a8dbb244b54c3de73a0997fcb611a3afd342590c32baf2f73545ce","throwable":""}
{"timestamp":"2021-04-28T18:54:22,730","level":"WARN","thread":"EthScheduler-Workers-3","class":"BlockPropagationManager","message":"Failed to import announced block 12330686 (0x61d53ccec97be310432f4c333254c143860fed70249b2cd8c8417b19993a8958).","throwable":""}
{"timestamp":"2021-04-28T18:54:22,759","level":"INFO","thread":"nioEventLoopGroup-3-10","class":"GetBlockFromPeerTask","message":"Failed to download block 0x61d53ccec97be310432f4c333254c143860fed70249b2cd8c8417b19993a8958 from peer Peer 0x4d305a8a834434b8c8....","throwable":""}
{"timestamp":"2021-04-28T18:54:22,800","level":"INFO","thread":"EthScheduler-Workers-2","class":"AbstractBlockProcessor","message":"Block processing error: transaction invalid 'NONCE_TOO_LOW'. Block 0x61d53ccec97be310432f4c333254c143860fed70249b2cd8c8417b19993a8958 Transaction 0x1cef0c4257a8dbb244b54c3de73a0997fcb611a3afd342590c32baf2f73545ce","throwable":""}
{"timestamp":"2021-04-28T18:54:22,800","level":"WARN","thread":"EthScheduler-Workers-2","class":"BlockPropagationManager","message":"Failed to import announced block 12330686 (0x61d53ccec97be310432f4c333254c143860fed70249b2cd8c8417b19993a8958).","throwable":""}
{"timestamp":"2021-04-28T18:54:23,748","level":"INFO","thread":"nioEventLoopGroup-3-1","class":"BlockPropagationManager","message":"Saving announced block 12330687 (0xbf26da0ba8e3f0caec39774368bbe460daf6de39632d6c71745a988929c62b26) for future import","throwable":""}
{"timestamp":"2021-04-28T18:54:24,878","level":"INFO","thread":"nioEventLoopGroup-3-8","class":"SyncTargetManager","message":"Found common ancestor with peer Peer 0x97b52d0754bcc1c9c4... at block 12330685","throwable":""}
{"timestamp":"2021-04-28T18:54:25,164","level":"INFO","thread":"EthScheduler-Services-380 (importBlock)","class":"AbstractBlockProcessor","message":"Block processing error: transaction invalid 'NONCE_TOO_LOW'. Block 0x61d53ccec97be310432f4c333254c143860fed70249b2cd8c8417b19993a8958 Transaction 0x1cef0c4257a8dbb244b54c3de73a0997fcb611a3afd342590c32baf2f73545ce","throwable":""}


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 11:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2204" class=".btn">#2204</a>
            </td>
            <td>
                <b>
                    Fix entropy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

 Use non-blocking randomness for acceptance tests

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 10:27:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2203" class=".btn">#2203</a>
            </td>
            <td>
                <b>
                    reduce blocks required for permissioning related tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is no reason to wait for 50 blocks. Reduce the number of blocks so tests run quicker

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 02:26:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2199" class=".btn">#2199</a>
            </td>
            <td>
                <b>
                    Add check to avoid useless modification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 13:51:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2197" class=".btn">#2197</a>
            </td>
            <td>
                <b>
                    fix selection of receive RPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are two RPC in Tessera for GET "/transaction/{hash}". This makes sure we are using the right one.

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>
 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 01:05:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2196" class=".btn">#2196</a>
            </td>
            <td>
                <b>
                    Removed container test build step.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamRevenant</span>
            </td>
            <td>
                Signed-off-by: Mark Terry <mark.terry@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
Removing the container test build step until the privacy issue is resolved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 21:21:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2193" class=".btn">#2193</a>
            </td>
            <td>
                <b>
                    Address 1559 config assumption
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                address assumption that if 1559 is enabled there is a london fork block config
fixes #2192

Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 23:47:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2185" class=".btn">#2185</a>
            </td>
            <td>
                <b>
                    Ignoring changelog modification on CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description

During releases we can waste time waiting for the pipeline while we only change the CHANGELOG. This PR will not run the tests if we only modify the CHANGELOG

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 13:45:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2184" class=".btn">#2184</a>
            </td>
            <td>
                <b>
                    fix GoQuorum privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The /receive RPC method that was used by Besu to retrieve private transactions in qoQuorum privacy mode from Tessera has been removed. This PR changes Besu to use the same RPC that is used by GoQuorum.

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 03:13:46 +0000 UTC
    </div>
</div>

