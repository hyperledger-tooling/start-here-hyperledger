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
                PR <a href="https://github.com/hyperledger/besu/pull/2224" class=".btn">#2224</a>
            </td>
            <td>
                <b>
                    fix goquorum privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes #2198
The bug was that when we have a private transaction in goquorum mode and a contract calls another contract or a contract deploys another contract the sender account from the public world state was used, which caused the nonce to be incremented in the public state. 

Signed-off-by: Stefan Pingel <stefan.pingel@consensys.net>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 01:58:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2223" class=".btn">#2223</a>
            </td>
            <td>
                <b>
                    Rayonism Branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull puts the rayonism branch we used for steklo into a hyperledger branch.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 01:46:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2222" class=".btn">#2222</a>
            </td>
            <td>
                <b>
                    update json-rpc responses for 1559
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/master/CONTRIBUTING.md -->

## PR description
* adds 1559-specific fields to json-rpc responses for BlockResult and TransactionResult
* removes empty gasPrice from TransactionResult from json-rpc serialization
* removes gasLimit from 1559 transactions json-rpc serialization
* fixes retesteth eth_getTransactionCount to use a hex rather than decimal for result

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #2215 
## Changelog

- [X] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 01:27:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2219" class=".btn">#2219</a>
            </td>
            <td>
                <b>
                    Test update 
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
        Created At 2021-05-04 15:06:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2218" class=".btn">#2218</a>
            </td>
            <td>
                <b>
                    PermissioningService Besu Plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # PermissioningService Besu Plugin

An additional plugin extension point has been added to besu to enable developers to intercept p2p connections and messages.

```java
public interface PermissioningService extends BesuPluginService {
  void registerNodePermissioningProvider(NodeConnectionPermissioningProvider provider);
  void registerNodeMessagePermissioningProvider(NodeMessagePermissioningProvider provider);
}
```

## NodeConnectionPermissioningProvider
This will allow plugin users to hook into node connections and when a node attempts to send messages using the following interface.
```java
@FunctionalInterface
public interface NodeConnectionPermissioningProvider {
  /**
   * Can be used to intercept the initial connection to a peer. Note that once a connection is
   * established it's bi-directional.
   *
   * @param sourceEnode the originators enode
   * @param destinationEnode the enode you are about to send to
   * @return if you can connect
   */
  boolean isConnectionPermitted(final EnodeURL sourceEnode, final EnodeURL destinationEnode);
}
```

## NodeMessagePermissioningProvider

If a provider has been registered through the plugin API all messages sent to a peer will use the hook to check if the message can be sent to a peer.

```java
@FunctionalInterface
public interface NodeMessagePermissioningProvider {
  /**
   * Can be used to intercept messages before they are sent from besu. 
   *
   * Note! this method is called on every message send.
   *
   * @param destinationEnode the enode you are about to send to
   * @param code devp2p code for the message
   * @return if we can send the message to the peer
   */
  boolean isMessagePermitted(final EnodeURL destinationEnode, final int code);
}
```
    

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-04 14:04:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2213" class=".btn">#2213</a>
            </td>
            <td>
                <b>
                    Ask block when not present
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

Two nodes stopped importing this weekend. This PR is a fix candidate. The nodes were late and some blocks were not stored in the pending blocks cache (because there is a size limit with announced blocks). At the time of importing the missing block, Besu did not find the block and stopped; Here is my theory. So I implemented a mechanism that directly asks the missing blocks to peers in these cases

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 14:13:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/2207" class=".btn">#2207</a>
            </td>
            <td>
                <b>
                    Fix GraphQL AT tests failing in GoQuorum mode.
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
Fix for GraphQL AT test failing due to incorrect schema in GoQuorum mode.

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 03:05:32 +0000 UTC
    </div>
</div>

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

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
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

