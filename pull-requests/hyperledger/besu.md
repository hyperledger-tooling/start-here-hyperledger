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
                PR <a href="https://github.com/hyperledger/besu/pull/5444" class=".btn">#5444</a>
            </td>
            <td>
                <b>
                    Update dependencies - commons-net
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Refs #5386 
This PR forces the commons-net version to be 3.9.0 but we can't do the same for antlr. antlr version needs to match the version in tuweni. So we need a tuweni release before we can update antlr.
This PR has the version we want but it's not yet released https://github.com/apache/incubator-tuweni/pull/479
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 05:40:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/5442" class=".btn">#5442</a>
            </td>
            <td>
                <b>
                    Fix for block import withdrawals
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
The initial intent of this PR was to fix the withdrawals field missing from the RawBlockIterator class used by the block import subcommand. Ended up introducing a refactor on some of the core methods of Block and BlockBody classes (readFrom and writeTo) aiming to remove duplicated code and reuse the existing logic defined in BlockBody.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Fixes #5431
It also fixes all the hive tests broken due to the impossibility of importing blocks (rpc-compat for example) that contained withdrawals via the `blocks import` subcommand.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 04:48:06 +0000 UTC
    </div>
</div>

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

PR does some plumbing to get TrieLogs and TrieLogFactory into the plugin-api, such that we can have a pluggable TrieLog serializer/deserializer and event observer.  Having trielogs in plugin-api also facilitates trielog push and pull to remote services.

notable changes/rearrangement:

* in plugin-api/services
  * adds TrieLogService 
  * adds plugin-api/services/trielog package:
    * TrieLog, now plugin interface for TrieLogLayer
    * TrieLog.LogTuple, now plugin interface for BonsaiValue
    * TrieLogEvent
    * TrieLogObserver
    * TrieLogAccumulator, now plugin interface for BonsaiWorldStateUpdateAccumulator

* in data types:
  * moves StorageSlotKey, into data-types
  * adds AccountValue, in data-types, now interface  for StateTrieAccountValue and BonsaiAccount
    
* writeRlp and writeInnerRlp moved from BonsaiValue into TrieLogFactory
* TrieLog now exposes the account, code, and storage maps directly rather than only via stream
    

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
fixes protocol-misc # 756
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
                <span class="chip">doc-change-required</span>
            </td>
            <td>
                ## PR description

Adds an option to send an SNI header on a TLS ClientHello message. Given the existing exposed options for the `TLSConfiguration`, I went for the `--Xp2p-tls-*` prefix for the new sni header option, instead of `p2p-tls-clienthello-sni` as it was stated in #4894 . Please let me know if you prefer otherwise.

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
- [x] have put X in the RPC name for now - spec may not be finalized
- [x] limit max number of user-specified constraints
- [x]  check expected storageHash against blockchainQueries actual value (needs a new method to expose this)

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

