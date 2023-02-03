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
                PR <a href="https://github.com/hyperledger/besu/pull/5047" class=".btn">#5047</a>
            </td>
            <td>
                <b>
                    Change param of to hexadecimal  of Eth fee history to match spec
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span><span class="chip">mainnet</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Change param type to accept hexadecimal and match the spec: https://ethereum.github.io/execution-apis/api-documentation/

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 11:54:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5046" class=".btn">#5046</a>
            </td>
            <td>
                <b>
                    4844 fix get blobls bundle v1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 11:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5045" class=".btn">#5045</a>
            </td>
            <td>
                <b>
                    Correctly set the fee market Cancun
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Fabio Di Fabio <fabio.difabio@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 11:33:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5044" class=".btn">#5044</a>
            </td>
            <td>
                <b>
                    Cancel older block creation tasks upon receiving a new one
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To avoid parallel block building on different threads, cancel any previous block building threads before starting a new one.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 11:16:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5042" class=".btn">#5042</a>
            </td>
            <td>
                <b>
                    Disable RocksDB checksum verification on reads
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 08:43:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5041" class=".btn">#5041</a>
            </td>
            <td>
                <b>
                    Move worldstate on forkchoice reorg
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: garyschulte <garyschulte@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
fix a latent issue where a reorg of the current chain head results in a mismatch between blockchain head and bonsai worldstate head

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #4784 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 01:03:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5039" class=".btn">#5039</a>
            </td>
            <td>
                <b>
                    Keep Worldstate Storage open for Bonsai archive latest layer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Fixes an issue where the latest block in BonsaiWorldStateArchive had a closed worldstate.  Persisting BonsaiInMemoryWorldState instances were creating entries in the archive with a snapshot worldstate that would subsequently be closed.  The net result was that queries using the worldstate for the `latest` block would frequently return Optional.empty() when accessing the closed worldstate.

this PR:
* uses a dedicated copy of the Bonsai in memory worldstate when creating a trielog
* adds a close() override to Bonsai layered worldstate to ensure the worldstate resources are cleaned up
* makes minor log change 


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes #5038 

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 01:56:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5037" class=".btn">#5037</a>
            </td>
            <td>
                <b>
                    Params should be single item of array type, not outer array of strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span><span class="chip">mainnet</span><span class="chip">EIP</span>
            </td>
            <td>
                See https://github.com/ethereum/execution-apis/issues/373
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 22:02:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5036" class=".btn">#5036</a>
            </td>
            <td>
                <b>
                    Rename JsonRpcService to EngineJsonRpcService
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

We have currently two JSON RPC services:
1) JsonRpcHttpService (used for regular API)
2) JsonRpcService (used for engine API)

While working on it, I often got confused between the two. The naming is almost identical and the classes are very alike. This PR renames `JsonRpcService` to `EngineJsonRpcService` to make it clearer where each service is used and to avoid confusions.

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 11:25:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5035" class=".btn">#5035</a>
            </td>
            <td>
                <b>
                    4844 re merge main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 11:04:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5030" class=".btn">#5030</a>
            </td>
            <td>
                <b>
                    T8n tool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Add t8n tool to evm tool.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 01:12:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5029" class=".btn">#5029</a>
            </td>
            <td>
                <b>
                    Fix for #3786 OOM on trace_block and trace_replayBlockTransactions RPC methods
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This change addresses a situation where all TraceFrame's for all Transactions in a block are loaded into memory, when only the TraceFrame's for a single Transaction are ever needed.

## Fixed Issue(s)
fixes #3786 

## Documentation
- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog
- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 20:48:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5027" class=".btn">#5027</a>
            </td>
            <td>
                <b>
                    Make rlp and hash strong references and precalculate children hashes for branch nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span>
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Make rlp and hash strong references and precalculate children hashes for branch nodes.
This is to reduce root hash calculation as we should keep more rlps and hashes in memory, but still need to check the memory footprint of this PR.

<img width="1700" alt="image" src="https://user-images.githubusercontent.com/5099602/215817606-b5b220f8-9b1a-4e2d-b7d7-8da1abcdb20a.png">


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 16:11:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5026" class=".btn">#5026</a>
            </td>
            <td>
                <b>
                    Improve withdrawals processing performance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">performance</span>
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
During withdrawals processing on devnet, profiling the execution showed two possible little improvements regarding performance.
<img width="1715" alt="image" src="https://user-images.githubusercontent.com/5099602/215738816-31ffd736-2982-4d3d-8e72-298bddbd6181.png">

The flamegraph at the block processing level

![image](https://user-images.githubusercontent.com/5099602/216040537-bd0cbbf1-f227-47a7-8e34-d2baec5aaf20.png)

With this PR, Withdrawals processing doesn't appear in the profiling flame graph (see below) which means it is faster than before. We can check also that the withdrawals are processed for each block with this log (see 16 ws for 16 withdrawals).
```
2023-01-31 14:21:24.413+00:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #28,191 / 0 tx / 16 ws / base fee 7 wei / 0 (0.0%) gas / (0x6a9b06fb18ffdae6377bd0d60d21a665df02c587393402e73cb2502eeda13cae) in 0.001s. Peers: 19
2023-01-31 14:21:37.092+00:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #28,192 / 0 tx / 16 ws / base fee 7 wei / 0 (0.0%) gas / (0x7c8060685283b172ed030cf8e7d7d609be61b16f58c2e49c493abceea80e572d) in 0.001s. Peers: 14
2023-01-31 14:21:48.651+00:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #28,193 / 0 tx / 16 ws / base fee 7 wei / 0 (0.0%) gas / (0x96494ca7da0cdc097a19f829f9decd16ed18b5d7f9d2c3920ca609a7936d09c3) in 0.001s. Peers: 14
2023-01-31 14:22:00.572+00:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #28,194 / 0 tx / 16 ws / base fee 7 wei / 0 (0.0%) gas / (0xb2f8c474e6f5d348b49269068cc0bd06da5affadd51411fb2eec56d5e59a58be) in 0.001s. Peers: 16
```

![image](https://user-images.githubusercontent.com/5099602/215786143-1a495973-a95a-43a4-93fe-d7f700da3057.png)

The flamegraph at the block processing level

![image](https://user-images.githubusercontent.com/5099602/216041247-ee3a7159-de45-45f8-93b0-2a056667284d.png)

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-31 10:47:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5023" class=".btn">#5023</a>
            </td>
            <td>
                <b>
                    Fix data gas calculation during block import
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 21:05:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5022" class=".btn">#5022</a>
            </td>
            <td>
                <b>
                    Re-merge main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 11:24:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5021" class=".btn">#5021</a>
            </td>
            <td>
                <b>
                    Add optional withdrawals to the NewPayload log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When withdrawals are null (i.e. disabled, pre-shanghai) then display nothing extra in the log.
When withdrawals are present, display their size, even when 0.

Chose 'ws' as a short name to keep the overall log small and since this is mostly useful for developers debugging rather than useful info for a node operator.

Tested on withdrawals-devnet-6, here's the Shanghai fork transition...
```
2023-01-30 20:53:44.059+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #304 / 0 tx / base fee 7 wei / 0 (0.0%) gas / (0x5d96179b829a1c2ba62774b9559a401b198375bc6d6b6a39521594ac6e5996e4) in 0.000s. Peers: 1
2023-01-30 20:53:44.818+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #305 / 0 tx / 0 ws / base fee 7 wei / 0 (0.0%) gas / (0x4199a28b76bc005897627cdbd7701e121be736c738294b1d09ccbb8291eadd2f) in 0.001s. Peers: 1
2023-01-30 20:53:46.078+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #306 / 0 tx / 0 ws / base fee 7 wei / 0 (0.0%) gas / (0xb68a8114d332339ec1e27cb53362626fa41e9a5ad6563334a6d181ea968f9211) in 0.000s. Peers: 1
2023-01-30 20:53:46.726+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #307 / 0 tx / 0 ws / base fee 7 wei / 0 (0.0%) gas / (0x66e995f758066e4abdbd1bb3928bd9bcd451b197d9eeb8b5c79de595508ec3d5) in 0.000s. Peers: 1
2023-01-30 20:53:47.008+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #308 / 0 tx / 0 ws / base fee 7 wei / 0 (0.0%) gas / (0xb93230252d104b6996b1e517ca766bbb157673270c5695a0c1608d98b616522a) in 0.001s. Peers: 3
2023-01-30 20:53:47.291+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #309 / 0 tx / 0 ws / base fee 7 wei / 0 (0.0%) gas / (0x152a3d68762b359abe5cb518567efc984445b588138a2cb8aee081c4692536f2) in 0.000s. Peers: 5
2023-01-30 20:53:47.839+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #310 / 0 tx / 0 ws / base fee 7 wei / 0 (0.0%) gas / (0xb79daa73a92dc261562488a012a9951cc67f2d95c0222b3b22d244686f475c8c) in 0.000s. Peers: 1
2023-01-30 20:53:48.552+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #311 / 0 tx / 0 ws / base fee 7 wei / 0 (0.0%) gas / (0xfb321669488d84e5fee40f3df6d6e904834ad2cec62051c920f70d9c31b8cf40) in 0.001s. Peers: 1
2023-01-30 20:53:48.722+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #312 / 0 tx / 0 ws / base fee 7 wei / 0 (0.0%) gas / (0x41e1cee974a10fd53dcdf663a7c231e7b0baf2ec8b8f246b0f9344a8fcebc612) in 0.001s. Peers: 1
2023-01-30 20:53:49.389+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #313 / 0 tx / 1 ws / base fee 7 wei / 0 (0.0%) gas / (0x9aef492f1e9833a0dd86aef0947032908b76c8fc4591aacea3b5d3e0791af93a) in 0.001s. Peers: 1
2023-01-30 20:53:49.820+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #314 / 0 tx / 11 ws / base fee 7 wei / 0 (0.0%) gas / (0x6fa79cb3ed0696dc8f94622accba4d86c137c56d7a23e709b8861b24b04ba678) in 0.003s. Peers: 1
2023-01-30 20:53:50.165+10:00 | vert.x-worker-thread-0 | INFO  | AbstractEngineNewPayload | Imported #315 / 0 tx / 16 ws / base fee 7 wei / 0 (0.0%) gas / (0x4773455ec25834ad1abe8f6ee107fa78bbd152ce6fc6f56acaa062ffda4e4154) in 0.001s. Peers: 2
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 10:57:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5020" class=".btn">#5020</a>
            </td>
            <td>
                <b>
                    Replace get by block number by get by block header
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
First batch that replaces getByBlockNumber by getByBlockHeader. These batch includes trivial replacements with none or minimal changes to the logic of the code base.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Partially fixes #4789

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 06:56:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5019" class=".btn">#5019</a>
            </td>
            <td>
                <b>
                    Add config option so that pos can be used at genesis
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Jason Frame <jason.frame@consensys.net>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Add a config option so that pos can be used from genesis. This is needed for some hive tests.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 16:02:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5018" class=".btn">#5018</a>
            </td>
            <td>
                <b>
                    Consumed data gas receipt fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-27 13:38:16 +0000 UTC
    </div>
</div>

