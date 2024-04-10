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
                PR <a href="https://github.com/hyperledger/iroha/pull/4415" class=".btn">#4415</a>
            </td>
            <td>
                <b>
                    [refactor] #4230: Remove `Domain::logo`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

Remove Domain::logo. Users who need it could store logo in domain metadata

### Linked issue

Closes #4230

### Checklist

- [x] I've read CONTRIBUTING.md
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 17:54:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4414" class=".btn">#4414</a>
            </td>
            <td>
                <b>
                    [ci]: Configure Sonarqube and Defectdojo in iroha2 CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
1. Substitute `llvm-cov` coverage tool by `grcov` (only `grcov` generates coverage reports that are compatible with Sonarqube).
2. Add jobs and steps into workflows to set up `lcov` and `clippy` reports uploading to Sonarqube and Defectdojo.
3. Bump `actions/checkout` somewhere.
4. Update `Dockerfiles.build`.

### Benefits
iroha2 dev code will be analyzed in Sonarqube and Defectdojo tools. Links to services URL will be provide in DM. It has access via corporate LDAP account.

### Note
It would be much better to send generared `clippy` and `lcov` reports from PR workflow where are they actually are generated. But we can't do it since GitHub actions security policies. So, we might try at least to upload them during pushing to dev branch. Hopefully, `dawidd6/action-download-artifact` has a magic to search for the latest uploaded artifact from the particular workflow.

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 13:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4413" class=".btn">#4413</a>
            </td>
            <td>
                <b>
                    [fix] #4253: Check genesis pub key in genesis round
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Verify that genesis transaction is indeed signed by genesis. 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4253 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Not possible to submit wrong genesis.

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
        Created At 2024-04-10 12:58:40 +0000 UTC
    </div>
</div>

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

