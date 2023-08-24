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
                PR <a href="https://github.com/hyperledger/iroha/pull/3835" class=".btn">#3835</a>
            </td>
            <td>
                <b>
                    [RFC]: on-chain scripting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 16:29:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3832" class=".btn">#3832</a>
            </td>
            <td>
                <b>
                    [feature] #3812 adding registerbox to DSL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Getting started on a syntax for `RegisterBox` to replace writing `RegisterBox::new(Domain::new("neverland".parse()?))` with `expr!(register "neverland")`, currently there's no way to describe objects which aren't domains. It also makes sense to separate the name detection logic from the DSL.

### Benefits

There's a consistent grammar across different kinds of resources like domains, assets, accounts which can be inferred when creating objects within the DSL. For instance, all assets will be `asset#domain`.

https://hyperledger.github.io/iroha-2-docs/guide/blockchain/naming.html

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] syntax for `register`
- [x] Domains
- [ ] Assets
- [ ] AssetDefinitions
- [ ] Accounts
- [ ] Moving detection code into separate crate
- [ ] CI checks

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-22 06:42:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3831" class=".btn">#3831</a>
            </td>
            <td>
                <b>
                    [fix] #3059: Simplify kura lock file code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3059  <!-- Replace with an actual number,  -->

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
        Created At 2023-08-21 18:29:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3830" class=".btn">#3830</a>
            </td>
            <td>
                <b>
                    [refactor] #3814: Update `iroha_ffi_derive` to use syn 2.0 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Separate parsing & (some) validation of attributes and codegen using `darling`, by storing this information into a strongly typed struct (`FfiTypeInput` and alike).

To facilitate this, add  parsers for `derive(FfiType)`, `getset` crate and built-in `repr` and `derive` attributes and tests for them.

One unfortunate concern is that now `ffi_derive` has stopped supporting unions completely, due to a limitation of `darling`. I don't think they are _that_ useful though, especially in context of a high level API iroha provides

### Linked issue

Closes #3814 

### Benefits

Cleaner code, better macro errors

### Checklist

- [x] Rebase (need less commits and proper messages)
- ~~[ ] Move utility classes to a common place (`iroha-derive-primitives`, probably)~~ not a good idea until `iroha-derive-primitives` is syn2-only
- [x] Make codegen for `ffi!`, `#[ffi_import]` and `#[ffi_export]` `emit!` errors rather than `bail!`ing
- [x] Clean up stray commented out code
- [x] Fix lints
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-21 15:07:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3827" class=".btn">#3827</a>
            </td>
            <td>
                <b>
                    [refactor] #3674: Elide `.cloned()` in `data_model/src/block.rs`
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
Get rid of unnecessary `iter::cloned()` call.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3674. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
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
        Created At 2023-08-21 08:00:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3824" class=".btn">#3824</a>
            </td>
            <td>
                <b>
                    [refactor] #3761: Rewrite `scripts/test-env.sh`
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
Rewrite the `test_env.sh` script as python. This should help with running it on systems that don't have bash as default due to python being more ubiquitous.
<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue
<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3761. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits
Slightly more descriptive docs and messages produced by the script, presumably increased readability.
<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] I've run the script with multiple configurations and with the oldest officially supported version of python to make sure it's sufficiently backwards compatible
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
        Created At 2023-08-18 17:53:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3823" class=".btn">#3823</a>
            </td>
            <td>
                <b>
                    [fix]: Update stable configs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
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
        Created At 2023-08-18 08:27:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3822" class=".btn">#3822</a>
            </td>
            <td>
                <b>
                    [fix]: Update stable configs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
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
        Created At 2023-08-18 08:26:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3821" class=".btn">#3821</a>
            </td>
            <td>
                <b>
                    [documentation] #3802: Unicode "kagami swarm" seed
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

A small Kagami help update

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

Closes #3802

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-18 07:53:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3820" class=".btn">#3820</a>
            </td>
            <td>
                <b>
                    [ci]: Fix permissions inside iroha2 Dockerfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
Fix permissions issue with rootless `iroha` user inside final Apline image.

### Benefits
Solve the problem with local docker deployment using repo's `docker-compose` files.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 14:41:35 +0000 UTC
    </div>
</div>

