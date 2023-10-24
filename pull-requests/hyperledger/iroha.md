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
                PR <a href="https://github.com/hyperledger/iroha/pull/4011" class=".btn">#4011</a>
            </td>
            <td>
                <b>
                    [fix] #3995: Fix topology mismatch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">Consensus</span>
            </td>
            <td>
                ## Description

Fix for bug with `TopologyMismatch`. 

Root cause for the problem was that after handling message peer state wasn't cleared.

In case if `view_change_index` of previous block was `1` than peer will submit block with wrong topology (because state is not cleared).
After reset new `Leader` would submit new block if this would arrive too late to `ProxyTail`, it would be corrupted without ability to recover. 

With current implementation of consensus it's troublesome to provide any test to verify that bug is 100% fixed...

I've created stand where i was able to successfully submit `263_975` blocks (run out of memory after that on my laptop).
Before the fix peers usually fail before that point (around `20_000` blocks or even earlier).

<details>
  <summary>Relevant logs</summary>  

  ```plain
2023-10-20T09:42:22.542288Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: View change updated addr=127.0.0.1:1340 role=ValidatingPeer current_view_change_index=1 <- VIEW CHANGE BIGGER THAN 1
2023-10-20T09:42:22.559937Z TRACE consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Block received, voting... addr=127.0.0.1:1340 role=ValidatingPeer block_hash=c421db0f81c31894d87af757f7cb3bcaba581405bdfe7f1ac6fc12d0ed78a7c5
2023-10-20T09:42:22.564224Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Block validated, signed and forwarded addr=127.0.0.1:1340 block_hash=c421db0f81c31894d87af757f7cb3bcaba581405bdfe7f1ac6fc12d0ed78a7c5
2023-10-20T09:42:22.585009Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Committing block addr=127.0.0.1:1340 role=ValidatingPeer block_height=20827 block_hash=934576a683136b0a87b6dfa65f43f1cc8416e8f8caf2e5d61d13a4fedd979903
2023-10-20T09:42:22.585900Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Creating block... txns=1 <- BLOCK IS CREATED WITHOUT RESET STATE
2023-10-20T09:42:22.588479Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Block created addr=127.0.0.1:1340 partial_hash=ecb2bafac04929924f4ccd7bea7705f73510e687088216a1b155e9fb1ab54a6f
2023-10-20T09:42:22.588882Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: View change updated addr=127.0.0.1:1340 role=Leader current_view_change_index=0 <- STATE IS RESET ONLY HERE
2023-10-20T09:42:22.588962Z TRACE consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Failed to add proofs into view change proof chain error=Block hash of proof doesn't match hash of proof chain
2023-10-20T09:42:22.589075Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Block sync update received addr=127.0.0.1:1340 role=Leader hash=934576a683136b0a87b6dfa65f43f1cc8416e8f8caf2e5d61d13a4fedd979903
2023-10-20T09:42:22.592757Z DEBUG consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Soft fork doesn't occurred: block has the same or smaller view change index addr=127.0.0.1:1340 role=Leader peer_latest_block_hash=Some({ iroha_crypto::hash::HashOf<iroha_data_mo
del::block::committed::VersionedCommittedBlock> 934576a683136b0a87b6dfa65f43f1cc8416e8f8caf2e5d61d13a4fedd979903 }) peer_latest_block_view_change_index=1 consensus_latest_block_hash=934576a683136b0a87b6dfa65f43f1cc8416e8f8caf2e5d61d13a4fedd979903 consensus_latest_block_view
_change_index=1
2023-10-20T09:42:22.592856Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Creating block... txns=1 
2023-10-20T09:42:22.594778Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Block created addr=127.0.0.1:1340 partial_hash=e6e7e50af9336376bbe711338076f1bde8c7708cc1748781af0239396e08a827 <- SECOND BLOCK CREATED FROM THE SAME LEADER
2023-10-20T09:42:22.601895Z TRACE consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Failed to add proofs into view change proof chain error=Block hash of proof doesn't match hash of proof chain
2023-10-20T09:42:22.601974Z ERROR consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: The hash of the committed block does not match the hash of the block stored by the peer. addr=127.0.0.1:1340 role=Leader committed_block_hash=(ecb2bafac04929924f4ccd7bea7705f7351
0e687088216a1b155e9fb1ab54a6f) voting_block_hash=e6e7e50af9336376bbe711338076f1bde8c7708cc1748781af0239396e08a827 <- AT THIS POINT IT'S TOO LATE BECAUSE PROXY TAIL COMMITTED WRONG BLOCK
2023-10-20T09:42:22.682569Z TRACE consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Failed to add proofs into view change proof chain error=Block hash of proof doesn't match hash of proof chain
2023-10-20T09:42:22.682706Z  INFO consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Block sync update received addr=127.0.0.1:1340 role=Leader hash=9ae7355147f52d40a088d0aa6d0b2a6c3b58a7c0b4119ed2caddd9e1e9dd7a31
2023-10-20T09:42:22.683046Z ERROR consensus:main_thread_cycle: iroha_core::sumeragi::main_loop: Block not valid. addr=127.0.0.1:1340 role=Leader block_hash=9ae7355147f52d40a088d0aa6d0b2a6c3b58a7c0b4119ed2caddd9e1e9dd7a31 error=TopologyMismatch { expected: UniqueVec([PeerId 
{ address: Ipv4(SocketAddrV4 { ip: Ipv4Addr([127, 0, 0, 1]), port: 1339 }), public_key: {digest: ed25519, payload: [3, 65, F, 57, B7, D9, 5D, 53, 33, E4, 5B, 2C, 25, C3, 76, F5, 28, 66, A0, D8, 70, 55, B3, 84, 69, 79, 5C, 87, D8, 36, D2, 6A]} }, PeerId { address: Ipv4(Socke
tAddrV4 { ip: Ipv4Addr([127, 0, 0, 1]), port: 1338 }), public_key: {digest: ed25519, payload: [10, 4D, E9, D3, A, 22, B4, AF, D0, 58, 28, 85, 8C, C2, 11, 29, 2E, 81, 85, D1, A1, 64, 66, B5, 8, 39, C6, 41, EB, 79, A7, 78]} }, PeerId { address: Ipv4(SocketAddrV4 { ip: Ipv4Add
r([127, 0, 0, 1]), port: 1337 }), public_key: {digest: ed25519, payload: [5C, 7, 84, 42, 2, E6, 5A, 8, AD, A0, D8, E9, 3, B8, 8B, AF, 7D, FE, 4, B0, B2, 7E, 6E, 42, D9, DF, D5, C, 32, 7F, 87, 54]} }, PeerId { address: Ipv4(SocketAddrV4 { ip: Ipv4Addr([127, 0, 0, 1]), port: 
1340 }), public_key: {digest: ed25519, payload: [6C, 50, 34, AE, BE, 12, F4, 97, C1, FB, BC, DA, C9, AC, C9, CA, D3, 45, 14, 94, 80, 3A, EC, 59, BE, FD, 42, DE, 1F, 3B, A6, AF]} }]), actual: UniqueVec([PeerId { address: Ipv4(SocketAddrV4 { ip: Ipv4Addr([127, 0, 0, 1]), port
: 1340 }), public_key: {digest: ed25519, payload: [6C, 50, 34, AE, BE, 12, F4, 97, C1, FB, BC, DA, C9, AC, C9, CA, D3, 45, 14, 94, 80, 3A, EC, 59, BE, FD, 42, DE, 1F, 3B, A6, AF]} }, PeerId { address: Ipv4(SocketAddrV4 { ip: Ipv4Addr([127, 0, 0, 1]), port: 1339 }), public_k
ey: {digest: ed25519, payload: [3, 65, F, 57, B7, D9, 5D, 53, 33, E4, 5B, 2C, 25, C3, 76, F5, 28, 66, A0, D8, 70, 55, B3, 84, 69, 79, 5C, 87, D8, 36, D2, 6A]} }, PeerId { address: Ipv4(SocketAddrV4 { ip: Ipv4Addr([127, 0, 0, 1]), port: 1338 }), public_key: {digest: ed25519,
 payload: [10, 4D, E9, D3, A, 22, B4, AF, D0, 58, 28, 85, 8C, C2, 11, 29, 2E, 81, 85, D1, A1, 64, 66, B5, 8, 39, C6, 41, EB, 79, A7, 78]} }, PeerId { address: Ipv4(SocketAddrV4 { ip: Ipv4Addr([127, 0, 0, 1]), port: 1337 }), public_key: {digest: ed25519, payload: [5C, 7, 84,
 42, 2, E6, 5A, 8, AD, A0, D8, E9, 3, B8, 8B, AF, 7D, FE, 4, B0, B2, 7E, 6E, 42, D9, DF, D5, C, 32, 7F, 87, 54]} }]) }
  ```
  
</details>

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3995  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Bug fixed.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-20 15:14:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4010" class=".btn">#4010</a>
            </td>
            <td>
                <b>
                    [fix]: #3898: Make `scripts/test_env.py` stop peers when aborting
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
The title is self-explanatory.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3898. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
Expected mode of termination on failure.
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
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
        Created At 2023-10-20 05:21:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4007" class=".btn">#4007</a>
            </td>
            <td>
                <b>
                    [feature] #3237: Expose cargo's output in wasm_builder_cli to have build progress information
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This adds a progress bar to `wasm_builder_cli` by exposing cargo's output (which already implements progress bar).

### Linked issue

Closes #3237 

### Benefits

The user can see the progress of the build

### Checklist

- [x] Make CI pass

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
        Created At 2023-10-19 07:31:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4004" class=".btn">#4004</a>
            </td>
            <td>
                <b>
                    [feature] #3130: Add type-state-pattern to divide client into sync and async parts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This PR adds traits to implement type-state-pattern on `Client` to divide it into sync and async parts.
I'm going to open also two pull requests:
- Add async client features
- `iroha_awc` and `iroha_hyper` crates implementations

### Linked issue

Closes #3130

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] Rewrite doc tests and examples
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs 

<!-- HINT:  Add more points to checklist for large draft PRs-->
- [ ] Open a pull request that adds async client features
- [ ] Open a pull request that add implementations of the `iroha_awc` and `iroha_hyper` crates

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 05:48:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4003" class=".btn">#4003</a>
            </td>
            <td>
                <b>
                    Paramtitle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span><span class="chip">api-changes</span><span class="chip">1.5</span>
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
        Created At 2023-10-17 22:14:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4002" class=".btn">#4002</a>
            </td>
            <td>
                <b>
                    [fix] #3971: Consensus bug fixes, RC20 backport
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
        Created At 2023-10-17 20:50:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4001" class=".btn">#4001</a>
            </td>
            <td>
                <b>
                    RC.20 Docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Let's update the Docker container names as we need to.
For the context, I left `hyperledger/` prefix in configurations that used it previously.
(What if somebody creates another `iroha2:dev` or `iroha2:stable` container on Dockerhub?)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-17 17:18:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3998" class=".btn">#3998</a>
            </td>
            <td>
                <b>
                    [ci] #3578: Add client cli tests into stable workflow
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

Update `Dockerfile.build.glibc`

Closes #3578 <!-- Replace with an actual number,  -->

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
        Created At 2023-10-17 15:54:36 +0000 UTC
    </div>
</div>

