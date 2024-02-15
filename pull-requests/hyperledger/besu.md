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
                PR <a href="https://github.com/hyperledger/besu/pull/6575" class=".btn">#6575</a>
            </td>
            <td>
                <b>
                    bump to 24.2.0-SNAPSHOT
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
post-release bump

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-15 00:20:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6574" class=".btn">#6574</a>
            </td>
            <td>
                <b>
                    Apply Reference tests v13.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Apply v 13.1 of the reference tests, includes test related fixes around initing the KZG precompile, uint64s in timestamps and blob gas, and some formatting cleanup.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 23:36:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6572" class=".btn">#6572</a>
            </td>
            <td>
                <b>
                    add a debug flavor of the openjdk-latest image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
As a user of the besu docker image I would like to have curl available in the running container.
As previous version openjdk-17 was also built in a debug flavor I followed this approach.

NB: teku include curl in their image https://github.com/Consensys/teku/blob/b544b9ebe589e78fa2f075ae389b041dc2871ea2/docker/jdk21/Dockerfile#L17

## Fixed Issue(s)
fixes #6571
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 15:12:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6570" class=".btn">#6570</a>
            </td>
            <td>
                <b>
                    remove useless persist during backward sync
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

During backward sync we call validateAndProcessBlock, which will process the block, update the state, and calculate the root hash.

If the block is validated, we will persist the block again for no reason, which will lead to a new unnecessary calculation of rootHash. Removing this second call should really significantly improve performance.


## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 14:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6568" class=".btn">#6568</a>
            </td>
            <td>
                <b>
                    Add tests for user profiles
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                Add tests to ensure that the profiles are sensible and besu will start with each of them

Refs #6323
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-14 04:25:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6563" class=".btn">#6563</a>
            </td>
            <td>
                <b>
                    Fix for tx incorrectly discarded when there is a timeout during block creation
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

In case the selection of transactions during block creation goes in timeout, it is possible that some txs are incorrectly dropped from the txpool, since marked as invalid.
When the timeout occurs the block is created with all the txs selected until that moment, after that the world state is closed, while it is possible that a tx was still processing, in that case the processing tx validation could fail due fact that is no more possible to get the account from the closed world state, and the tx is wrongly tagged as invalid with UPFRONT_COST_EXCEED_BALANCE, that cause the tx to be dropped from the pool.

This PR, improves the handling of timeout and not selected txs, avoiding that them can be incorrectly dropped in case of timeout

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 13:37:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6562" class=".btn">#6562</a>
            </td>
            <td>
                <b>
                    feat: add fixed basefee options
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
Add `fixedBaseFee` options to forced `baseFee` same as `gasPrice` value.


I'm new to the Java language, please guide any aspects I can further improve or modify.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
https://github.com/hyperledger/besu/issues/6335
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 11:15:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6561" class=".btn">#6561</a>
            </td>
            <td>
                <b>
                    Bonsai limit trie logs enabled true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ux</span>
            </td>
            <td>
                Swap default value for --Xbonsai-limit-trie-logs-enabled from false to true

Also added a fallback value for the option (otherwise specifying --Xbonsai-limit-trie-logs-enabled on the command line, without a value, has the opposite effect

builds on #6536 

This option is not yet documented so no docs changes required.

Breaking change
The limit is now enabled by default. If you do not want the limit enabled, you need to explicitly set it to false
--Xbonsai-limit-trie-logs-enabled=false

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-13 04:19:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6559" class=".btn">#6559</a>
            </td>
            <td>
                <b>
                    [Issue 6301] Refactor BadBlockManager
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
Refactor `BadBlockManager` handling - move it out of `ProtocolSpec` and into `ProtocolContext`.  This will make it simpler to expose bad block events through the plugins API.  

This refactor simplifies access to `BadBlockManager` and improves the clarity of the codebase. Accessing `BadBlockManager` through `ProtocolSpec` is misleading because it implies this object is changing depending on the current spec / milestone.  However, this is not the case - `BadBlockManager` is a global cache unrelated to the spec. 

Now, instead of accessing the `BadBlockManager` in a roundabout way by pulling the latest spec:
```
Blockchain chain = protocolContext.getBlockchain();
BlockHeader head = chain.getChainHeader()
BadBlockManager badBlockManager = protocolSchedule
        .getByBlockHeader(head)
        .getBadBlocksManager()
``` 
You can just grab it directly from `ProtocolContext.getBadBlockManager()`. 

**Notes for the reviewer**:
The first commit moves the instantiation of `BadBlockManager` from `ProtocolScheduleBuilder` to `BesuControllerBuilder`.  This introduces a lot of changes because `BadBlockManager` now has to be injected into `ProtocolScheduleBuilder`.  The second commit pushes `BadBlockManager` into `ProtocolContext`, which also introduces a lot of changes - mostly in tests.  The rest of the commits are much smaller and more manageable. 

## Fixed Issue(s)
Part of #6301 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-12 22:18:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6558" class=".btn">#6558</a>
            </td>
            <td>
                <b>
                    Remove uses of org.jetbrains annotations
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

We have a mix of org.jetbrains.annotations.NotNull and javax.annotations.Nonnull. Change all to the latter. Add an errorprone check to enforce this.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-10 19:37:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6557" class=".btn">#6557</a>
            </td>
            <td>
                <b>
                    Move account warming from gas calculator to call operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

The BerlinGasCalculator had a side effect of warming addresses when calculating call gas costs. By introducing a boolean we can keep the side effects in the operation instead of in the gas calculator. This makes gas cost estimation by downstream users of the API safer.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 19:38:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6555" class=".btn">#6555</a>
            </td>
            <td>
                <b>
                    Database metadata refactor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

Besu storage could have different formats, currently Forest or Bonsai, and each format can have different versions. We used to have only one identifier for these two properties, but this is not optimal, for clarity and does not play well with the fact that the storage is implemented via plugins.

Besu should only know about the format, and tell the plugin which is the required format, then the version of the format is something internal to the plugin itself.

So I moved the `DataStorageFormat` to the plugin API project, and this is the reason for the many file changed, most of them are just changes to reflect this move.
Then inside the RocksDB plugin I introduced the new class `VersionedStorageFormat` to managed the versioning of RocksDB databases.

The database metadata file, reflects this change, having an entry for the format and one for the version, for example, the default Bonsai storage will have this metadata (note the versioning of the metadata itself `v2` object, so we can introduce a `v3` if needed in future): 
```
{
  "v2": {
    "format": "BONSAI",
    "version": 2
  }
}
```

To correct the missed introduction of the new version, when the variables storage format was introduced, now for both Forest and Bonsai, a new version has been introduced, the version `2` for each format, being `1` the version pre variables storage.

At startup the existing metadata, that we call `v1` format, is automatically translated to the new format.

Check have been added to detect not managed (up|down)grades, so we can inform the user of the right steps, if the process in not automated.

Test to perform:

- [x] Vanilla new installation, verify that the default format and version is used and written in DATABASE_METADATA.json 
- [ ] New installation with custom format selection, verify that the selected format and version is used and written in DATABASE_METADATA.json 
- [ ] Upgrade existing installation >=23.4.4, verify that DATABASE_METADATA.json has been translated to the new format
- [ ] Upgrade existing installation >=23.4.4 then downgrade, verify that after the downgrade Besu refuses to start since the metadata is not recognized
- [ ] Upgrade existing installation >=23.4.4 then revert metadata, then downgrade, verify that after the downgrade Besu starts correctly
- [ ] Upgrade existing installation <23.4.4, verify that variables storage migration is performed and DATABASE_METADATA.json has the new format
- [ ] Upgrade existing installation <23.4.4 then downgrade, verify that after the downgrade Besu refuses to start since the metadata is not recognized
- [ ] Upgrade existing installation <23.4.4 then revert metadata, then downgrade, verify that after the downgrade Besu starts correctly
## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #6408 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 11:33:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6551" class=".btn">#6551</a>
            </td>
            <td>
                <b>
                    use terminal width for usage message
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ux</span>
            </td>
            <td>
                fixes #6429
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 05:12:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6550" class=".btn">#6550</a>
            </td>
            <td>
                <b>
                    Uprev24.1.2
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 05:07:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6549" class=".btn">#6549</a>
            </td>
            <td>
                <b>
                    Uprev24.1.2
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 04:48:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6548" class=".btn">#6548</a>
            </td>
            <td>
                <b>
                    uprev artifact name
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-09 03:10:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6546" class=".btn">#6546</a>
            </td>
            <td>
                <b>
                    Blob gas fee checking
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes: #6391 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 15:56:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6545" class=".btn">#6545</a>
            </td>
            <td>
                <b>
                    timestamp set for dencun on mainnet.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Timestamp set for cancun on mainnet.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 15:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6541" class=".btn">#6541</a>
            </td>
            <td>
                <b>
                    disable privacy tests since they are currently flaky
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These tests are flaky right now for 2 reasons, and work is in progress to fix. 

See 

Run tessera as a process (currently using docker) for ATs https://github.com/hyperledger/besu/pull/5968

Also occasionally errors since the txpool is disabled during initial sync - it's been somewhat [mitigated](https://github.com/hyperledger/besu/pull/6479) but hasn't totally fixed it
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 02:51:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6540" class=".btn">#6540</a>
            </td>
            <td>
                <b>
                    rocksdb usage - Replace Column Size with more accurate Total Size
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">TeamGroot</span>
            </td>
            <td>
                Replace "Column Size" with "Total Size" where Total Size = SST Files Size + Blob Files Size

`besu storage rocksdb usage`

e.g. with a BONSAI + X_SNAP node...

BEFORE THIS PR

```
| Column Family                  | Keys            | Column Size  | SST Files Size  |
|--------------------------------|-----------------|--------------|-----------------|
| BLOCKCHAIN                     | 2355141414      | 905 GiB      | 166 GiB         |
| VARIABLES                      | 26              | 120 KiB      | 240 KiB         |
| ACCOUNT_INFO_STATE             | 9634454         | 294 MiB      | 496 MiB         |
| ACCOUNT_STORAGE_STORAGE        | 24041432        | 977 MiB      | 1 GiB           |
| CODE_STORAGE                   | 37703864        | 10 GiB       | 12 GiB          |
| TRIE_BRANCH_STORAGE            | 1885032116      | 110 GiB      | 138 GiB         |
| TRIE_LOG_STORAGE               | 267301          | 14 GiB       | 17 GiB          |
```

Column Size Total =  905 + 0.294 + 0.977 + 10 + 110 + 14 = 1042 GB

AFTER THIS PR

```
| Column Family                  | Keys            | Total Size  | SST Files Size  | Blob Files Size  |
|--------------------------------|-----------------|-------------|-----------------|------------------|
| BLOCKCHAIN                     | 2355141414      | 933 GiB     | 166 GiB         | 767 GiB          |
| VARIABLES                      | 26              | 240 KiB     | 240 KiB         | 0 B              |
| ACCOUNT_INFO_STATE             | 9634454         | 496 MiB     | 496 MiB         | 0 B              |
| ACCOUNT_STORAGE_STORAGE        | 24041432        | 1 GiB       | 1 GiB           | 0 B              |
| CODE_STORAGE                   | 37703864        | 12 GiB      | 12 GiB          | 0 B              |
| TRIE_BRANCH_STORAGE            | 1885032116      | 138 GiB     | 138 GiB         | 0 B              |
| TRIE_LOG_STORAGE               | 267301          | 17 GiB      | 17 GiB          | 0 B              |
|--------------------------------|-----------------|-------------|-----------------|------------------|
| ESTIMATED TOTAL                | 4311820607      | 1104 GiB    | 337 GiB         | 767 GiB          |
```

1104 GB is much closer to the on disk result:

```
$du -ksch /data/besu/database
1.1T	/data/besu/database
1.1T	total
```

---

Another example with a BONSAI + X_CHECKPOINT node:

```
| Column Family                  | Keys            | Total Size  | SST Files Size  | Blob Files Size  |
|--------------------------------|-----------------|-------------|-----------------|------------------|
| BLOCKCHAIN                     | 1432578448      | 685 GiB     | 101 GiB         | 583 GiB          |
| VARIABLES                      | 4970            | 89 KiB      | 89 KiB          | 0 B              |
| ACCOUNT_INFO_STATE             | 236237895       | 11 GiB      | 11 GiB          | 0 B              |
| ACCOUNT_STORAGE_STORAGE        | 1112465479      | 49 GiB      | 49 GiB          | 0 B              |
| CODE_STORAGE                   | 37702404        | 12 GiB      | 12 GiB          | 0 B              |
| TRIE_BRANCH_STORAGE            | 1853480673      | 134 GiB     | 134 GiB         | 0 B              |
| TRIE_LOG_STORAGE               | 514             | 69 MiB      | 69 MiB          | 0 B              |
|--------------------------------|-----------------|-------------|-----------------|------------------|
| ESTIMATED TOTAL                | 4672470383      | 893 GiB     | 309 GiB         | 583 GiB          |
```

```
$ du -ksch /data/besu/database
896G	/data/besu/database
896G	total
```

---

Also dumping a bunch of stats out in...
`besu storage rocksdb stats`

which is useful for seeing the blobdb garbage stats (useful for https://github.com/hyperledger/besu/pull/6289#pullrequestreview-1851948029) among other things.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 02:26:39 +0000 UTC
    </div>
</div>

