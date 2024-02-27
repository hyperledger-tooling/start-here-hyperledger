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
                PR <a href="https://github.com/hyperledger/iroha/pull/4326" class=".btn">#4326</a>
            </td>
            <td>
                <b>
                    [fix] #4287: use `algorithm` in `PrivateKey` serialized form
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">config-changes</span><span class="chip">UI</span><span class="chip">crypto</span>
            </td>
            <td>
                ## Description

Aligns serialized form of `PrivateKey` with its representation in Rust, i.e. rename `digest_function` to `algorithm`.

This change might cause compatibility issues, but let's consider them as a part of the overall breaking configuration change: #2585 

### Linked issue

Closes #4287


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 21:46:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4319" class=".btn">#4319</a>
            </td>
            <td>
                <b>
                    [feature] #3660: Add Numeric type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

Introduce unified decimal numeric type for assets, no more `Quantity`, `BigQuantity`, `Fixed`.

Type is represented as `96bit` mantissa + `scale` up to 28 decimal places.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3660 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Simplified code, decimals commonly use in monetary applications.

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
        Created At 2024-02-22 11:57:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4318" class=".btn">#4318</a>
            </td>
            <td>
                <b>
                    Update CODEOWNERS: remove Kshitij Roodkee
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                As @0x009922 requested Kshitij Roodkee to be removed from `CODEOWNERS`: Kshitij would contribute, but he's busy with his new internship, as far as I am aware.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 07:47:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4316" class=".btn">#4316</a>
            </td>
            <td>
                <b>
                    [ci]: Unsync auto-labels. Fix `config-changes` condition
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

1. The bot was observed to remove a label manually added to PR: https://github.com/hyperledger/iroha/pull/4309#issuecomment-1958760549
2. At the same time, the bot was observed to notify false-positive `config-changes` due to its wrong definition
	- Closes #4278
<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

1. Always prioritize manual labeling/unlabeling
2. Necessary and sufficient `config-changes` notifications

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
        Created At 2024-02-22 06:27:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4313" class=".btn">#4313</a>
            </td>
            <td>
                <b>
                    [fix] #4311: fix pre-commit hook
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description
the `pre-commit` hook still generates the genesis in `peer` even though it does not exist anymore after the big change in the configuration

### Linked issue

Closes #4311

### Checklist

- [X] I've read `CONTRIBUTING.md`
- [X] I've used the standard signed-off commit format (or will squash just before merging)
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
        Created At 2024-02-21 07:21:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4310" class=".btn">#4310</a>
            </td>
            <td>
                <b>
                    [refactor] #3901: delete NewParameter isi and use only SetParameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ## Description
`NewParameter` is only used during genesis generation. it does not make sense to have it as ISI. Now the admin will generate the parameters during configuration and he can give permessions for other users to allow them to put parameters. 

### Linked issue


Closes #3901

### Checklist

- [X] I've read `CONTRIBUTING.md`
- [X] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-21 06:58:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4309" class=".btn">#4309</a>
            </td>
            <td>
                <b>
                    [feature] #4212: Prevent account registration without signatures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #4212 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

More logical

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
        Created At 2024-02-20 21:38:55 +0000 UTC
    </div>
</div>

