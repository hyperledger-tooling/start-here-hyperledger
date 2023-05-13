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
                PR <a href="https://github.com/hyperledger/iroha/pull/3477" class=".btn">#3477</a>
            </td>
            <td>
                <b>
                    [fix] #3233: Remove duplicated error messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">UI</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3233 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Old error message:

```
Error: Transaction rejected

Caused by:
   0: Transaction was rejected: Transaction rejected due to insufficient authorisation: Action not permitted: Validator denied the operation `SignedTransaction { payload: TransactionPayload { account_id: admin@admin, instructions: [TransferBox { source_id: AssetId(rose##alice@wonderland), object: 1_u32, destination_id: AccountId(admin@admin) }], creation_time: 1683932346090, time_to_live_ms: 100000, nonce: None, metadata: {} }, signatures: {iroha_crypto::signature::SignatureOf<iroha_data_model::transaction::model::TransactionPayload>({ pub_key: ed0120419AAFB36674C689D2B612EC6903364DDDB0CE8FF0F4031D8E3F8ACE88F42B5F, payload: 9ACCE845B6CD44ED13A14915528B3F09BECFF36E14765D426A0276F9B986340513B7B8CB7D2CB3DC9C080387EEA81472DCA5EA37E3E7C7BD2465D9A0B275B50D })} }`: `Can't transfer assets of another account`
   1: Transaction rejected due to insufficient authorisation: Action not permitted: Validator denied the operation `SignedTransaction { payload: TransactionPayload { account_id: admin@admin, instructions: [TransferBox { source_id: AssetId(rose##alice@wonderland), object: 1_u32, destination_id: AccountId(admin@admin) }], creation_time: 1683932346090, time_to_live_ms: 100000, nonce: None, metadata: {} }, signatures: {iroha_crypto::signature::SignatureOf<iroha_data_model::transaction::model::TransactionPayload>({ pub_key: ed0120419AAFB36674C689D2B612EC6903364DDDB0CE8FF0F4031D8E3F8ACE88F42B5F, payload: 9ACCE845B6CD44ED13A14915528B3F09BECFF36E14765D426A0276F9B986340513B7B8CB7D2CB3DC9C080387EEA81472DCA5EA37E3E7C7BD2465D9A0B275B50D })} }`: `Can't transfer assets of another account`
   2: Action not permitted: Validator denied the operation `SignedTransaction { payload: TransactionPayload { account_id: admin@admin, instructions: [TransferBox { source_id: AssetId(rose##alice@wonderland), object: 1_u32, destination_id: AccountId(admin@admin) }], creation_time: 1683932346090, time_to_live_ms: 100000, nonce: None, metadata: {} }, signatures: {iroha_crypto::signature::SignatureOf<iroha_data_model::transaction::model::TransactionPayload>({ pub_key: ed0120419AAFB36674C689D2B612EC6903364DDDB0CE8FF0F4031D8E3F8ACE88F42B5F, payload: 9ACCE845B6CD44ED13A14915528B3F09BECFF36E14765D426A0276F9B986340513B7B8CB7D2CB3DC9C080387EEA81472DCA5EA37E3E7C7BD2465D9A0B275B50D })} }`: `Can't transfer assets of another account`
```

New error message:

```
Error: Transaction was rejected

Caused by:
   0: Validation failed
   1: Not permitted
   2: Validator denied the operation [TRANSFER `1` FROM `rose##alice@wonderland` TO `admin@admin`] by `admin@admin`
   3: Can't transfer assets of another account
```

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Further work

We should return a more detailed error from validator. I.e. it should explain on which instruction validation of transaction failed.
Also we should try to avoid using `Trap` because hard to work with when trying to analyze errors.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2023-05-12 23:02:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3476" class=".btn">#3476</a>
            </td>
            <td>
                <b>
                    [fix] #3462: Add burn asset command to client_cli
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
        Created At 2023-05-12 08:56:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3475" class=".btn">#3475</a>
            </td>
            <td>
                <b>
                    [feature] #2373: `kagami swarm`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

_It is still a draft_

### Linked issue

Closes #2373

### Benefits

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

### TODO

- [ ] Define all consts (like `docker-compose.yml`, `config` dir, `iroha-clone` dir, iroha repo etc)
- [ ] Don't serialize empty `command` field (now it is `command: null`)
- [ ] Get git revision in the same way as main Iroha CLI does (remove `git-version` dependency)
- [ ] Remove Dockerhub support?
- [ ] UI: implement prompting (using `unquiry`)
- [ ] UI: add logging throughout the process. Add spinner (using `spinoff`) during the long-running processes, like validator compilation
- [ ] Fix rest of Iroha according to updates in `ConfigurationProxy`
- [ ] #3473: Support standalone validator compilation
- [ ] Finish unit tests
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-12 08:31:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3474" class=".btn">#3474</a>
            </td>
            <td>
                <b>
                    [fix] #3444: Remove custom discriminants from scale encoding
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
        Created At 2023-05-12 07:03:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3460" class=".btn">#3460</a>
            </td>
            <td>
                <b>
                    Update MAINTAINERS.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Let's update the maintainer list, adding Alexander Strokov and Michael Timofeev.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 04:44:30 +0000 UTC
    </div>
</div>

