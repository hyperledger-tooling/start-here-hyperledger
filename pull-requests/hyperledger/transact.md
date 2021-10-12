---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    Release notes for 0.3.11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 15:01:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    Backport 0-3: stabilize "state-merkle-sql"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change back-ports the following PRs:

* #189
* #191
* #192  
* #193 
* #209 
* #214
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 17:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    stabilize "state-merkle-sql"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR also stabilizes "sqlite" and "postgres" features. 

It also includes a new test run to cover the postgres tests with the stable feature group enabled. This run is executed only in CI.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 15:50:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/213" class=".btn">#213</a>
            </td>
            <td>
                <b>
                    Update various dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 21:43:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/212" class=".btn">#212</a>
            </td>
            <td>
                <b>
                    Fix `time_to_wait` comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix out of date comments related to the `time_to_wait` arg.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 16:36:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Merge insert nodes and update changelog operations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 14:38:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    Add duration to workload command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add a `--duration` option to the workload CLI command that allows a user to set the amount of time in hours that a workload should run for, this value can be provided in seconds, minutes, hours, or days. ex: 7s, 20m, 24h, 2d

### Testing:
1. Start two splinter nodes and create a circuit
2. Updload the command or smallbank smart contract
3. Start a workload using the transact CLI:
```
cargo run --manifest-path cli/Cargo.toml \
  --features=experimental workload \
  --key <private_key_file_path> \
  --workload command \
  --targets http://localhost:8080/scabbard/<circuit_id>/<service_id> \
  --target-rate 1/s \
  -vv \
  --update 2 \
  --duration 10s
```
The workload should run for the duration given and then exit, shutting down the workload.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-07 17:02:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/209" class=".btn">#209</a>
            </td>
            <td>
                <b>
                    Replace OverlayReader/Writer with MerkleRadixStore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR replaces the OverlayReader/Writer with a MerkleRadixStore trait.  The SqlMerkleRadixStore implementation of this trait isolates all of the operations usage behind the trait, and allows for all of the operations, schema's and models to be moved into a store module.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-06 17:11:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/208" class=".btn">#208</a>
            </td>
            <td>
                <b>
                    Update migration log to be debug and include crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrea Gunderson <agunde@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-05 18:42:22 +0000 UTC
    </div>
</div>

