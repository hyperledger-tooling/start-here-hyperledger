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

- [ ] Vanilla new installation, verify that the default format and version is used and written in DATABASE_METADATA.json 
- [ ] New installation with custom format selection, verify that the selected format and version is used and written in DATABASE_METADATA.json 
- [ ] Upgrade existing installation >=23.4.4, verify that DATABASE_METADATA.json has been translated to the new format
- [ ] Upgrade existing installation >=23.4.4 then downgrade, verify that after the downgrade Besu refuses to start since the metadata is not recognized
- [ ] Upgrade existing installation <23.4.4, verify that variables storage migration is performed and DATABASE_METADATA.json has the new format
- [ ] Upgrade existing installation <23.4.4 then downgrade, verify that after the downgrade Besu refuses to start since the metadata is not recognized


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
                
            </td>
            <td>
                Replace "Column Size" with "Total Size" where Total Size = SST Files Size + Blob Files Size

`besu storage rocksdb usage`

BEFORE THIS PR

```
| Column Family                  | Keys            | Column Size  | SST Files Size  |
|--------------------------------|-----------------|--------------|-----------------|
| BLOCKCHAIN                     | 1428244409      | 654 GiB      | 101 GiB         |
| VARIABLES                      | 3114            | 10 KiB       | 115 KiB         |
| ACCOUNT_INFO_STATE             | 235049771       | 8 GiB        | 11 GiB          |
| ACCOUNT_STORAGE_STORAGE        | 1111008228      | 38 GiB       | 49 GiB          |
| CODE_STORAGE                   | 37676523        | 9 GiB        | 12 GiB          |
| TRIE_BRANCH_STORAGE            | 1842206479      | 105 GiB      | 132 GiB         |
| TRIE_LOG_STORAGE               | 515             | 30 MiB       | 77 MiB          |
```

Column Size Total =  654 + 8 + 38 + 9 + 105 = 814 GB

AFTER THIS PR

```
| Column Family                  | Keys            | Total Size  | SST Files Size  | Blob Files Size  |
|--------------------------------|-----------------|-------------|-----------------|------------------|
| BLOCKCHAIN                     | 1428245080      | 681 GiB     | 101 GiB         | 580 GiB          |
| VARIABLES                      | 3121            | 115 KiB     | 115 KiB         | 0 B              |
| ACCOUNT_INFO_STATE             | 235050819       | 11 GiB      | 11 GiB          | 0 B              |
| ACCOUNT_STORAGE_STORAGE        | 1111009063      | 49 GiB      | 49 GiB          | 0 B              |
| CODE_STORAGE                   | 37676523        | 9 GiB       | 12 GiB          | 0 B              |
| TRIE_BRANCH_STORAGE            | 1842217975      | 132 GiB     | 132 GiB         | 0 B              |
| TRIE_LOG_STORAGE               | 516             | 77 MiB      | 77 MiB          | 0 B              |
```

Total Files Size Total =  681 + 11 + 49 + 12 + 132 = 885 GB

885 GB is much closer to the on disk result:

```
du -ksch /data/besu/database
889G	/data/besu/database
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6539" class=".btn">#6539</a>
            </td>
            <td>
                <b>
                    Fix checkLicense gradle task
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
I'm getting a gradle build failure due the "checkLicenses" task.  This looks like a misspelling:
```
% ./gradlew dev -x test

FAILURE: Build failed with an exception.

* What went wrong:
Task 'checkLicenses' not found in root project 'besu' and its subprojects. Some candidates are: 'checkLicense'.
```

Fix this by using the existin "checkLicense" task.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-08 00:04:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6537" class=".btn">#6537</a>
            </td>
            <td>
                <b>
                    Github Actions Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Uses `pull_request_target` to make sure action definitions only come from `main` or `release-*`. This also allows them to escalate privs.
- All priv escalations moved as narrowly as possible. Typically this is only required to upload test results.
- All actions pinned to specific SHA versions. When updated, repository settings will need to be adjusted to allow it.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 17:39:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6536" class=".btn">#6536</a>
            </td>
            <td>
                <b>
                    Default storage format now Bonsai 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                Builds on #6530 
Refs #5391 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-07 02:26:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6534" class=".btn">#6534</a>
            </td>
            <td>
                <b>
                    [minor] Improve message when existing database is different from the configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ux</span>
            </td>
            <td>
                ## PR description

Improve message error when existing database with a different version is detected

`Mismatch: DB at '/path' is FOREST (Version 1) but config expects BONSAI (Version 2). Please check your config.`

see: #5926
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 13:10:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6533" class=".btn">#6533</a>
            </td>
            <td>
                <b>
                    Add missing javadoc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Add missed javadoc for `ClassicEVM` from #6524
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 12:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6530" class=".btn">#6530</a>
            </td>
            <td>
                <b>
                    Make SNAP the default sync mode for named networks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                refs #5391
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 09:00:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6528" class=".btn">#6528</a>
            </td>
            <td>
                <b>
                    error if snap or checkpoint sync specified with privacy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                we enforce that you can't specify FAST sync if privacy is enabled - do the same check for SNAP and CHECKPOINT
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 06:23:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6526" class=".btn">#6526</a>
            </td>
            <td>
                <b>
                    Acceptance Tests - only run non-privacy ATs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span>
            </td>
            <td>
                exclude privacy tests since they are currently flaky (they are run on a separate nightly cadence)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 01:33:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6525" class=".btn">#6525</a>
            </td>
            <td>
                <b>
                    Better tracing alignment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Update tracing and evm tool
* Intrinsic gas is optional in EVMTool
* For call series, also charge the gas given to the next call level

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

Fixes #6523
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 00:23:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6524" class=".btn">#6524</a>
            </td>
            <td>
                <b>
                    Add ETC Spiral EVM configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
During the last ETC network upgrade, Besu nodes got stalled because, inadvertently, [EIP-4399](https://eips.ethereum.org/EIPS/eip-4399) was _included_ instead of _omitted_.

For the future, we'll also test omissions to the protocol and not only additions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-05 05:14:33 +0000 UTC
    </div>
</div>

