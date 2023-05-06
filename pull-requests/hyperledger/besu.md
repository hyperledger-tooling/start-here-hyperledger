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
                PR <a href="https://github.com/hyperledger/besu/pull/5440" class=".btn">#5440</a>
            </td>
            <td>
                <b>
                    TrieLogFactory plugin support
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

Draft PR currently.  PR does some plumbing to get TrieLogs and TrieLogFactory into the plugin-api

notable changes/rearrangement:
    TrieLog, now plugin interface for TrieLogLayer
    TrieLog.LogTuple, now plugin interface for BonsaiValue
    TrieLogEvent
    TrieLogObserver
    TrieLogAccumulator, now plugin interface for BonsaiWorldStateUpdateAccumulator
    StorageSlotKey, now in data-types
    AccountValue, in data-types, now interface  for StateTrieAccountValue and BonsaiAccount
    
  writeRlp and writeInnerRlp moved from BonsaiValue into TrieLogFactory
  TrieLog now exposes the account, code, and storage maps directly rather than only via stream
    
Creating a TrieLogService BesuService will be the last addition, still outstanding

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-06 02:35:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5439" class=".btn">#5439</a>
            </td>
            <td>
                <b>
                    Add option to send SNI header in TLS ClientHello message [#4894]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Adds an option to send an SNI header on a TLS ClientHello message. Given the existing exposed options for the `TLSConfiguration`, I went for the `--Xp2p-tls-*` prefix for the new sni header option, in contrast to how it was stated in #4894 . Please let me know if you prefer otherwise.

* add --Xp2p-tls-clienthello-sni option to enable the SNI header

## Fixed Issue(s)
fixes hyperledger#4894
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 09:59:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5438" class=".btn">#5438</a>
            </td>
            <td>
                <b>
                    Enable blobs on Blockchain and trie log column families
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
Enable blobs on Blockchain and trie log column families.
Only values that are bigger than 4 KiB are written to Blobs

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 09:09:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5436" class=".btn">#5436</a>
            </td>
            <td>
                <b>
                    Send rawtx conditional
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Related to account abstraction. 

Implementation of this endpoint https://notes.ethereum.org/@yoav/SkaX2lS9j
* basically the same as eth_sendRawTransaction, with the ability to specify a number of conditions
* have put X in the RPC name for now - spec may not be finalized
* TODO check expected storageHash against blockchainQueries actual value (needs a new method to expose this)
* TODO In case of repeated failures or knownAccounts too large, the error code SHOULD be -32005 (Limit exceeded) with a description of the error
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 05:24:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5434" class=".btn">#5434</a>
            </td>
            <td>
                <b>
                    Txpool save restore
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

With this PR a new option (`--tx-pool-enable-save-restore`) is available, disabled by default, so current behavior is not changed, and when enabled it causes the txpool to save it content on file on shutdown and reloading it on startup, this is particularly useful to not lose locally submitted transactions during a restart, but could also useful to quickly warmup the txpool on restarts, without waiting for a good number of peers.
From benchmark on a `m6a.xlarge` saving a txpool with 100000 transactions, takes less that a seconds, so it does not affect shutdown time, and restoring just few seconds, and it is done async, so it does not affect the startup time as well.

On shutdown the content is save in a file, then after the reload is complete the file is deleted. By default the save file is located in the data dir, and named `txpool.dump`, but if needed it is possible to specify another path for the file with the option `--tx-pool-save-file`.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 19:00:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5432" class=".btn">#5432</a>
            </td>
            <td>
                <b>
                    fix certs for PKCS11 acceptance tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Some tests started failing because of expired certificates. This PR fixes that
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 11:09:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5430" class=".btn">#5430</a>
            </td>
            <td>
                <b>
                    Eip 6780 selfdestruct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Wire in a check to see if an account is new in the TX scope
* Create a new SelfDestruct Opcode that only deletes accounts
  that register as new within tx scope.

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 21:27:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5429" class=".btn">#5429</a>
            </td>
            <td>
                <b>
                    Move Big EOF out of Cancun
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move the implementation of "big" eof into Future EIPs, out of cancun. Also, create space for Prague, Osaka, and Bogota forks in the EVM code.

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
        Created At 2023-05-03 19:08:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5428" class=".btn">#5428</a>
            </td>
            <td>
                <b>
                    Fix the number of RocksDB log files to 5 with 100 MB each
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ameziane H <ameziane.hamlat@consensys.net

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Fix the number of RocksDB LOG files to 5 with 100 MB for each LOG file.
These logs are not to be confused with [number].log files which represent WAL files.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 10:19:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5426" class=".btn">#5426</a>
            </td>
            <td>
                <b>
                    Fix RocksDB missing metrics issue
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
I noticed that RocksDB metrics are no more exposed even when they are enabled.
This is a regression on main branch, this PR will fix this issue.

![image](https://user-images.githubusercontent.com/5099602/235882942-2f251d5d-8fd8-4cff-a51d-76e3d5665719.png)

## Fixed Issue(s)
#5427
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 09:37:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5425" class=".btn">#5425</a>
            </td>
            <td>
                <b>
                    Ban zero blob transactions
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

[An update to EIP-4844](https://github.com/ethereum/EIPs/pull/6863) made zero blob transactions invalid, so this PR adds the check to verify that at least one blob is specified, this check could be done statically when creating the transaction.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

fixes #5401 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 09:30:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5424" class=".btn">#5424</a>
            </td>
            <td>
                <b>
                    Acceptance Test for Shanghai EVM changes (push0)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #5403

Splits Shanghai AT test cases out from paris.
Idea is to have an AT per "fork transition", i.e. ExecutionEngineShanghaiAcceptanceTest for paris -> shanghai
next one would be ExecutionEngineCancunAcceptanceTest for shanghai -> cancun
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 08:45:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5423" class=".btn">#5423</a>
            </td>
            <td>
                <b>
                    Remove block creation task map entries when cancelling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Fixes potential memory leak - probably only significant for clients running lots of validators

## Testing

- [x] beku-timestamp with validators
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 07:12:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5422" class=".btn">#5422</a>
            </td>
            <td>
                <b>
                    Certificates - specify long expiry for intermediate certs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">testing</span><span class="chip">dev experience</span>
            </td>
            <td>
                -validity 36500 needs to be specified for -gencert as well as -genkeypair

other changes to README are cosmetic

TODO - run through these commands to regenerate the certs used by the unit tests (suspect ATs may have the same problem - maybe we have not hit this issue there since they are running on nightly cadence)

see #5421 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-03 06:38:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5419" class=".btn">#5419</a>
            </td>
            <td>
                <b>
                    Update sonarcloud.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Update actions versions

Add workflow_dispatch


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 21:40:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5418" class=".btn">#5418</a>
            </td>
            <td>
                <b>
                    Transaction pool flag to disable specific behaviors for locally submitted transactions
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

Setting the option `tx-pool-disable-locals` transactions submitted via API `eth_sendrawtransaction` do not receive a special treatment and are validated like any remote transactions, and are not prioritized over remote transactions.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 19:45:06 +0000 UTC
    </div>
</div>

