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
                PR <a href="https://github.com/hyperledger/iroha/pull/4203" class=".btn">#4203</a>
            </td>
            <td>
                <b>
                    [feature] #4183: change endpoint to return single matching transaction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Update endpoint that returned `Vec<SignedTransaction>` to return `Option<SignedTransaction>` instead.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4183 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
It decreases the amount of traffic through the network and removes the necessity for the batching of the pending transactions.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2024-01-16 19:40:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4201" class=".btn">#4201</a>
            </td>
            <td>
                <b>
                    [refactor]: Fix CI lints after bump of toolchain version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Fixed CI lints

`missing_panics_doc` now fires for every public function that calls `Option::expect` or `Result::expect`. In some cases (like `Metadata`) I've extracted the panicking into a special private function because I don't think it's a good solution to just slap `missing_panics_doc` on every function that asserts invariants. We definitely want to get rid of these warnings, but what to do about it?

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
        Created At 2024-01-15 09:03:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4200" class=".btn">#4200</a>
            </td>
            <td>
                <b>
                    [refactor] #4167: asset subcommand in client CLI to be consistent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

In asset subcommand in the CLI operations like `mint`, `burn`, `get`, `transfer` had `register`. I refactored the subcommand to follow the suggestions in #4167.

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4167

<!-- Link if e.g. JIRA issue or  from another repository -->

### Use cases

#### Register
```bash
./iroha_client_cli asset  --definition-id="tea#looking_glass" --value-type=Quantity 
```
#### Mint
```bash
./iroha_client_cli asset mint --asset-id="tea##mad_hatter@looking_glass" --quantity="100"
```
#### Burn
```bash
./iroha_client_cli asset burn --asset-id="tea##mad_hatter@looking_glass" --quantity="10"
```

#### Get
```bash
./iroha_client_cli asset get --asset-id="tea##mad_hatter@looking_glass"  
```
#### Transfer
```bash
./iroha_client_cli asset transfer --to="white_rabbit@looking_glass" --asset-id="tea##mad_hatter@looking_glass" --quantity="5"  
```
### Checklist

- [X] I've read `CONTRIBUTING.md`
- [X] I've used the standard signed-off commit format (or will squash just before merging)
- [X] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 12:53:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4198" class=".btn">#4198</a>
            </td>
            <td>
                <b>
                    [fix] #4162: SignedTransaction is immutable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Remove `payload_mut` method which is considered harmful.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4162 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Don't break `SignedTransaction` invariant.

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
        Created At 2024-01-12 10:57:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4196" class=".btn">#4196</a>
            </td>
            <td>
                <b>
                    [ci] #4184: Bump to 2024-01-12 toolchain & Revert to custom Coveralls settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
1. Update `iroha2ci-image` to the latest nightly toolchain (`2024-01-12`).
2. Bump `ci-contaier` in workflows to `hyperledger/iroha2-ci:nightly-2024-01-12`
3. Revert to the custom base branch comparison for Coveralls

### Linked issue
#4184 #4131 

### Benefits
1. Use the freshest rust nightly toolchain in CI
2. Attempt to normalize the Coveralls work

### IMPORTANT NOTE
Since we have updated the ci-image, WE MUST build and push it before the actual workflows will start to use it in CI. Previously we did it outside iroha repo (usually from forks) using the special HL DockerHub credentials that Hyperledger provided to us. Unfortunately, as Ry Jones told, they decided to remove these credentials since they can't continue to pay for that. Thus, we must to build and push the new ci-image asap when this PR will be merged.

### UPD
Ry Jones decided to give us one more year for external HL DockerHub account. So, the new ci-image 
has been already pushed from my fork.

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
        Created At 2024-01-12 09:12:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4193" class=".btn">#4193</a>
            </td>
            <td>
                <b>
                    [fix] #4192: Fix musl archiver name in Docker
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Fix was successfully tested by @timofeevmd 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #4192 <!-- Replace with an actual number,  -->

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
        Created At 2024-01-11 16:31:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4191" class=".btn">#4191</a>
            </td>
            <td>
                <b>
                    [refactor] #4152: Remove `bridge` and `dex` features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Remove obsolete features not used anywhere in the project.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4152 <!-- Replace with an actual number,  -->

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
        Created At 2024-01-11 07:35:35 +0000 UTC
    </div>
</div>

