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
                PR <a href="https://github.com/hyperledger/iroha/pull/4411" class=".btn">#4411</a>
            </td>
            <td>
                <b>
                    [feature] #2085: Authenticate personal accounts by ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

#### [feature] #2085: Authenticate personal accounts by ID

This is a milestone for the following commit. The inclusion of the public key in the ID allows the ID to match the verifying key of the signature. This makes it possible to authenticate transactions and queries with the ID alone.

- `api-changes`: single signatory account, single signature transaction
- `api-changes`: remove query `FindAccountsByName`
- `config-changes`: client config `account.id` changes to `account.domain_id`
- add `iroha_sample_params` utility for tests
- different notions of signatories "peer", "genesis", and "alice" in the test network

#### [feature] #2085: Auto-register destination account on transfer

Includes registration of the destination account in the transfer execution. The main use case is described in test `auto_register_account::on_transfer::asset_numeric`

### Linked issue

- This is the 1st of the 3-part work of account restructuring:
  - Closes #2085
  - #4372
  - #4373
- Opens #4410
- Contains suggestions for #4409

### Benefits

As long as you know the address (account ID), you can send without worrying whether the destination account is already registered on the chain.
However, the current design requires the sender to be authorized to register a new account within the domain. See https://github.com/hyperledger/iroha/pull/4411#discussion_r1552269607

### Drawbacks

- Conventional `name@domain` notation will be temporary lost
  - For dev use, introduces an utility `iroha_sample_params::alias`
  - To be restored with #4372
- Multi-signature functionality will be temporary lost, coupled with [the queue change](https://github.com/hyperledger/iroha/pull/4308)
  - To be restored and enhanced with #4373

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [x] I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 18:22:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4408" class=".btn">#4408</a>
            </td>
            <td>
                <b>
                    [feature] #4093, #4110: Add public key mint and burn commands to `iroha_client_cli`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- Add a client CLI command for adding a new signatory to an account (minting a public key for an account).
- Add a client CLI command for burning a public key from an account.

### Linked issue

Closes #4093 and #4110.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-04 07:17:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4407" class=".btn">#4407</a>
            </td>
            <td>
                <b>
                    [fix] #4242: Remove permissions from roles on entity unregistration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Since roles are mutable now, we can remove permission tokens from them as well as from accounts. 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4242 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

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
        Created At 2024-04-03 14:05:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4406" class=".btn">#4406</a>
            </td>
            <td>
                <b>
                    [fix] #4403: Trigger metadata is accessible in smart contracts (BACKPORT)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- .metadata() now available in user code
- CanSetKeyValueInTrigger and CanRemoveKeyValueInTrigger properly handled

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4403 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

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
        Created At 2024-04-03 13:44:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4405" class=".btn">#4405</a>
            </td>
            <td>
                <b>
                    [fix] #4403: Trigger metadata is accessible in smart contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- `.metadata()` now available in user code
- `CanSetKeyValueInTrigger` and `CanRemoveKeyValueInTrigger` properly handled

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4403 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

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
        Created At 2024-04-03 13:43:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4404" class=".btn">#4404</a>
            </td>
            <td>
                <b>
                    [fix] #4307: Pad `r` and `s` to 32 bytes in `secp256k1_sign` test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Currently, the `signature::secp256k1::test::secp256k1_sign` test fails intermittently due to `r` sometimes producing a vector of 31 bytes instead of 32, which makes `EcdsaSecp256k1Sha256::verify` fail on the total `r + s` length check (==64). 

Maybe it's possible that `s` does the same, so I padded `s` too to be safe – but I don't have the cryptography background to confirm that (failing cases have pointed to `r` only). I'm also unaware if it's possible for `r` or `s` to be >32 bytes long.

### Linked issue

Closes #4307.

### Benefits

Test should no longer be flaky.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up
### 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 12:45:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4402" class=".btn">#4402</a>
            </td>
            <td>
                <b>
                    [refactor] #4289: Use `nonzero!` instead of fallible NonZero* constructors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Replace fallible or unsafe constructor invocations of non-zero numeric types with the macro from `nonzero_ext` where possible.

### Linked issue

Closes #4289.

### Benefits

Invalid constants are caught at compile time. Unnecessary unsafe code removed.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 07:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4401" class=".btn">#4401</a>
            </td>
            <td>
                <b>
                    [refactor] #4290: Replace `parse_display` crate with `strum`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Remove the `parse_display` dependency since `strum` provides the needed derives.

### Linked issue

Closes #4290.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 11:31:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4400" class=".btn">#4400</a>
            </td>
            <td>
                <b>
                    [fix] #4397: Make queue tests use a mock time source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This PR adds a `TimeSource` to `iroha_primitives` - a mockable time source. It then proceeds to make the queue tests use the mock time source to make them deterministic.

### Linked issue

Closes #4397

### Benefits

- less flaky CI
- ability to mock transaction times (useful [here](https://github.com/hyperledger/iroha/pull/4382#discussion_r1540619904))

### Checklist

- [ ] make CI pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-01 09:30:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4398" class=".btn">#4398</a>
            </td>
            <td>
                <b>
                    [fix] #4267: Introduce p2p idle timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

Previously iroha tried to connect indefinitely to idle peer.

Introduce idle timeout for p2p communication:

Each peer track the last time it received message (or ping) from particular peer, if this time is larger than timeout peer is disconnected.

If no other messages were produced in time equal to half timeout ping is send to prove that peer isn't idle.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4267 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### How to test

1. setup iroha network with multiple peers using `LOGLEVEL=TRACE ./scripts/test_env.py setup`
2. kill one of the peers (e.g. iroha1)
3. start listening on p2p port this peer was using `nc -l 1338`
4. check that peers terminate connection with this "peer" after timeout

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
        Created At 2024-03-29 11:21:27 +0000 UTC
    </div>
</div>

