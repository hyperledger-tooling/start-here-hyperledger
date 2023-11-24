---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4076" class=".btn">#4076</a>
            </td>
            <td>
                <b>
                    [fix] #4063: update configuration endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

I've implemented the changes according to the linked issue:

- Remove documentation retrieval from the API
- Normalize DTO structure with the configuration file

### Linked issue

Closes #4063 

### Benefits

A little step closer to implementing the Configuration RFC (#2585).

### Checklist

- [x] I've written unit tests for the code changes
- [x] Self-review
- [x] Open corresponding PR updating the docs
  - https://github.com/hyperledger/iroha-2-docs/pull/435
- [x] Write an integration test
- [x] Remove redundant `Result<bool>`
- [ ] Use `PATCH` instead of `POST`

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 06:35:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4073" class=".btn">#4073</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4065: Prevent pub key spoofing in p2p
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Backport for recently merged #4069

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 11:59:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4071" class=".btn">#4071</a>
            </td>
            <td>
                <b>
                    [fix] #4070: Enable `tls-rustls-native-roots` `iroha_client` feature by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Deploying behind an HTTPS proxy seems like a common occurrence, so we should have some TLS implementation by default.

Rustls brings less problems with linking under musl, so use it

### Linked issue

Closes #4070

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Make a sane choice so that the user does not have to. If they don't like the choice, they can disable the default features and make their own.

### Checklist

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 10:51:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4069" class=".btn">#4069</a>
            </td>
            <td>
                <b>
                    [fix] #4065: Prevent pub key spoofing in p2p
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">Security</span>
            </td>
            <td>
                ## Description

Instead of sending just pub key it's now required to send pub key + signature of shared session key to prove ownership of this public key in order to prevent spoofing.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4065 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Security bug resolved.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-22 08:37:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4066" class=".btn">#4066</a>
            </td>
            <td>
                <b>
                    [fix] #0000: fix stable client config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-21 09:10:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4062" class=".btn">#4062</a>
            </td>
            <td>
                <b>
                    [feature] #4060: add support for boxed slices in FFI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4060

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 15:29:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4061" class=".btn">#4061</a>
            </td>
            <td>
                <b>
                    [refactor] #2664: Introduce new wsv
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">Optimization</span>
            </td>
            <td>
                ## Description

Introduce new in memory storage for iroha. 

New approach provide single reader, multiple readers where readers don't block writers and writer doesn't block readers. 

Single writer seems reasonable restriction since only single block is processed at the same time. 

Instead of single `WorldStateView` multiple transactions are now used.

Work is based on [`concread`](https://github.com/kanidm/concread) crate.

```mermaid
graph TD;
    WS-->WSV;
    WS-->WSB;
    WSB-->WST;
    WST-->WSS;
    WSV-->WSS;

    WS["State"]
    WSV["StateView"]
    WSB["StateBlock"]
    WST["StateTransaction"]
    WSS["StateSnapshot"]
```

- `State` in-memory iroha storage
- `StateView` read-only snapshot of state at some point in time
- `StateBlock` aggregate state changes during block execution (need commit to take effect)
- `StateTransaction` aggregate state changes during transaction execution (need commit to take effect)
- `StateSnapshot` used to convert view and transaction to the same read-only type. 


<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #2664 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Faster on large larger state
- Readers and writer are independent

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Benchmark results

Iroha tps benchmark was used. In this bechmark only small fraction of state is changed with single transaction (imo it's reasonable to expect that single transaction won't change whole state).

Genesis was generated with the following command: 

```bash
cargo run --bin kagami genesis --domains 250 --accounts-per-domain 100 --assets-per-domain 100 > configs/peer/genesis.json 
```
This command creates genesis about 400 Mb in size.


Set the following config for `clients/bench/config.json`

```json
{
    "peers": 1, // 4 -> 1 To speed up things
    "interval_us_per_tx": 0,
    "max_txs_per_block": 1024,
    "blocks": 15,
    "sample_size": 10,
    "genesis_max_retries": 1200 // Wait for large genesis to be committed
}
```

Than bench two times before and after changes in wsv.

```
export WSV_WASM_RUNTIME_CONFIG='{ "FUEL_LIMIT": 18446744073709551615, "MAX_MEMORY": 4294967295 }'
cd client
cargo run --release --example tps-oneshot
```

tps-oneshot results: 

Before update: tps=3.3077273188803833
After update: tps=2339.2057925660447

To measure memory consumption heaptrack was used. 

Allocation sizes and amounts:

Before:

![before](https://github.com/hyperledger/iroha/assets/40040452/eeb85c99-e85a-44ff-9a50-1fd18ee0a40a)

After:

![after](https://github.com/hyperledger/iroha/assets/40040452/0d38bd98-5507-420b-a65a-eb76a15337a0)

All relevant files: [link](https://drive.google.com/drive/folders/1AeagOk7KeO5VE2nTAPDNUSw4XZAT8APw).

### TODO

- [ ]: Create relevant issues
- [ ]: Rename no longer relevant variable names, update docs, ...

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 14:40:27 +0000 UTC
    </div>
</div>

