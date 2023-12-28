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
                PR <a href="https://github.com/hyperledger/iroha/pull/4181" class=".btn">#4181</a>
            </td>
            <td>
                <b>
                    [refactor] #4045: Use concrete key types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">Security</span>
            </td>
            <td>
                ## Description

- `PublicKey` and `PrivateKey` are now enums with explicit key types. No invalid state is possible
- Fixed some tests
- Fixed now useless signatures of depended code
- Fixed some clippy lints

## TODO

Currently it's impossible to build Executor or any wasm, because used crypto libraries are feature-gated, meaning that even `PublicKey` and `PritateKey` cannot be represented as is in WASM.

Solutions I see:

- Let WASM have all crypto code and remove feature-gate. Unused code will likely be optimized by Rust, but I'm not sure.
- Have another `PublicKey` and `PrivateKey` for WASM types which will be compatible with types from Host in terms of encoding and serialization

For any of this solutions I would like to hear other opiniont, especially from @mversic .

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #4045
- Openned #4174 

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- More robust solution because now we are sure that stored keys are valid
- No more errors are possible when creating keys or signing
- Test are more real now

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

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
        Created At 2023-12-28 16:12:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4180" class=".btn">#4180</a>
            </td>
            <td>
                <b>
                    [fix] #4177: Fixed (get|set)_config 401 HTTP.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                

## Description

Added Client's headers to the requests

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

* Closes #4177  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [x] I replied to all comments after code review, marking all implemented changes with thumbs up

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
        Created At 2023-12-28 12:24:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4179" class=".btn">#4179</a>
            </td>
            <td>
                <b>
                    [BACKPORT]: Fix smart contract debug print
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-27 15:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4178" class=".btn">#4178</a>
            </td>
            <td>
                <b>
                    [fix] #0000: Fix smart contract debug print
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-27 15:14:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4175" class=".btn">#4175</a>
            </td>
            <td>
                <b>
                    [feature] #3974: Add subcommands into iroha_client_cli to edit domain metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Fork of #4054 with a small update to from_str method

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3974  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

There won't be any confusions about why the same method for different structs implemented differently

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
        Created At 2023-12-25 19:43:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4173" class=".btn">#4173</a>
            </td>
            <td>
                <b>
                    Trying to repair dependency which stopped working (protoc for golang)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span><span class="chip">build</span><span class="chip">dependencies</span>
            </td>
            <td>
                ## Description
During working on PR (https://github.com/hyperledger/iroha/pull/4003) unfortunately dependency (not connected with the PR) stopped working. Inside the PR it can't be repaired "Pull requests from forks are not allowed to change Dockerfiles", so I'm trying to correct its from another branch of main iroha repository (not fork)

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
Iroha Hyperledger 1 starts compiling again

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
        Created At 2023-12-25 16:44:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4172" class=".btn">#4172</a>
            </td>
            <td>
                <b>
                    [fix] #0000: Use free port in test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Use free port in integration test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-25 13:39:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4171" class=".btn">#4171</a>
            </td>
            <td>
                <b>
                    [fix] #4155: ensure the secp256k1 signatures coming out of OpenSSL are normalized
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This is an interoperability problem between OpenSSL and newer cryptographic libraries, see [BIP-0062](https://github.com/bitcoin/bips/blob/master/bip-0062.mediawiki#user-content-Low_S_values_in_signatures) for details

This fixes the flaky secp256k1_sign test

Also includes a drive-by cleanup of useless `assert(result.is_ok())`

### Linked issue

Closes #4155

### Benefits

Fixes the flaky test! Less flaky tests is obviously better 

### Checklist

- [ ] make ci pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-25 11:53:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4170" class=".btn">#4170</a>
            </td>
            <td>
                <b>
                    [refactor] #3068: remove flattened events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This PR removes duplicated flattened events. Those are events like the `DataEvent::Account(_)` and `DataEvent::Asset(_)`. They are already present under other event types (`DataEvent::Domain(DomainEvent::Account(_))`, for example) and were duplicated to simplify the event filter construction (?).

While an immediate effect of this change is ever more increased amount of boilerplate to construct event filters, this provides a more orthogonal events system, helping to build a comprehensive DSL.

### Linked issue

Partially addresses #3068 

### Checklist

- [x] make ci pass
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-25 08:48:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4169" class=".btn">#4169</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4164: Fix topology update on restart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                Backport of #4165.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-25 07:43:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4168" class=".btn">#4168</a>
            </td>
            <td>
                <b>
                    [refactor]: update iroha_telemetry_derive to use syn2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Update with refactoring to remove proc_macro_error in favour of our `Emitter` wrapper

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3909 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->


### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
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
        Created At 2023-12-25 03:22:07 +0000 UTC
    </div>
</div>

