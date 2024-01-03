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

Currently it's impossible to build Executor or any wasm, because used crypto libraries are feature-gated, meaning that even `PublicKey` and `PrivateKey` cannot be represented as is in WASM.

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

