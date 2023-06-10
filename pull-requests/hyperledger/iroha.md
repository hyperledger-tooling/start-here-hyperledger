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
                PR <a href="https://github.com/hyperledger/iroha/pull/3599" class=".btn">#3599</a>
            </td>
            <td>
                <b>
                    [feature] #3597: Permisison Token Analysis (Iroha side)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

This PR is based on PR #3588 branch, so most of the code diff is not related directly no this PR.

So, please, review only the latest commit.

I plan to merge this after #3588.

- Implemented a new state for `wasm::Runtime` related to `permission_tokens()` *Validator* entrypoint
- Added execution of this new entrypoint
- Added permission tokens replacement in `Upgrade<Validator>` execution

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3597  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Support for permission token analysis on Iroha side

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

## When undraft?

- After the merge of #3588 

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
        Created At 2023-06-10 15:40:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3593" class=".btn">#3593</a>
            </td>
            <td>
                <b>
                    [fix] #3592: fix config files updating on release
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

Closes #3592 

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
        Created At 2023-06-09 10:49:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3589" class=".btn">#3589</a>
            </td>
            <td>
                <b>
                    [fix] #0000:  configuration macro test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Update failing `configuration_proxy_from_env_returns_err_on_parsing_error` test.

### Linked issue

_No linked issue_

### Checklist

- [x] I've run tests locally

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-09 04:46:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3588" class=".btn">#3588</a>
            </td>
            <td>
                <b>
                    [feature] #3587: Allow different states in wasm::Runtime & link-time …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

- Added support for different state types into `Runtime`
- Added support for `state` attribute into `iroha_wasm_codec_derive`, so that there will be a way to specify state type when it's unable to infer it from parameters
- Added different `wasmtime::Linker` configurations for different states

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

* Closes #3587  <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Ability to expand state types which I'm blocked with in #3230 
- Link-time checking for inappropriate function calls from WASM

See issue description for more details.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
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
        Created At 2023-06-08 23:30:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3586" class=".btn">#3586</a>
            </td>
            <td>
                <b>
                    [documentation]: remove Kagami documentation from README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

After a discussion with the team, we decided that it is better to not have Kagami documentation in README than having an outdated one. Since it is a CLI tool with no stable API, having reliable help message (thanks to `clap`) is enough.

See https://github.com/hyperledger/iroha/issues/3509#issuecomment-1581766055

### Linked issue

_No issue_

### Benefits

Lower chance to have outdated documentation in the README. Therefore, lower chance to confuse future users.

### Checklist

- [ ] Peers review

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 01:48:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3585" class=".btn">#3585</a>
            </td>
            <td>
                <b>
                    [feature] #2373: `kagami swarm file` and `kagami swarm dir`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

#3475 introduces `kagami swarm` command, but it works only in directory mode. Now it is possible to produce both a "battery-included" directory and just a single file. The latter usage is especially helpful to generate sample docker-compose configurations to store them in the repo (`docker-compose.yml`, `docker-compose.single.yml` etc):

```bash
# only `docker-compose.yml`
kagami swarm file ./docker-compose.yml --build . --config-dir ./configs/peer --p 4 --seed "Kagami"

# a whole directory `test-swarm`
kagami swarm dir ./test-swarm --build . -p 4 --seed "Kagami"
```

### Linked issue

Closes #2373

### Benefits

We can automatise Docker Compose configurations generation and avoid problems with having outdated files in the repo. It will help the community.

### Checklist

- [x] Remove `--outfile` and `--outdir` options, use positionals instead
- [ ] Create an issue to include compose files generation into CI
- [x] Self-review

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-08 00:25:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3575" class=".btn">#3575</a>
            </td>
            <td>
                <b>
                    [ci] #3562: Fix PR-generator Jenkinsfile & Add Coverall badge & Set up JDK 11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
1. Change `README.MD` badge from `Codecov` to `Coveralls` tool.
2. Update PR-generator `Jenkinsfile`.
3. Add `docker.soramitsu.co.jp/iroha2/iroha2:dev-${{ github.event.pull_request.head.sha }}` iroha2 image tag to push to Soramitsu registry for PR-generator.
4. Add JDK distribution to `Set up JDK 11` step into `java-api` job inside `I2::Release::Tests` workflow.

### Linked issue
1. We don't have `Coveralls` coverage tool badge.
2. PR-generator deployment hasn't bee finished.
3. #3562 

### Benefits
1. `Coveralls` badge.
2. PR-generator should work after merging the corresponding PR with Jenkins library (I'LL NOTIFY WHEN IT WILL BE ABLE TO BE TESTED)!
3. Fix JDK 11 Set up in the `Release-PR` workflow.

### Checklist

- [X] Done the work
- [X] CI checks pass
- [X] Commits are good
- [ ] Addressed comments
- [ ] Tested badge as UI element. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-07 14:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3572" class=".btn">#3572</a>
            </td>
            <td>
                <b>
                    [fix] #3162: Forbid 0 height in block streaming request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Use `NonZeroU64` for block streaming to prevent user from sending 0 as block height.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3162 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Clear error.

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
        Created At 2023-06-06 19:37:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3571" class=".btn">#3571</a>
            </td>
            <td>
                <b>
                    [fix] #3546: Fix time trigger tests get stuck
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Change order in which we submit first transaction and start listening for events.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3546 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Test doesn't get stuck.

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
        Created At 2023-06-06 15:49:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3563" class=".btn">#3563</a>
            </td>
            <td>
                <b>
                    [feature] #3088: Introduce queue throttling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Instead of introducing separate queue for MST transaction and double required space for queue. 
It was decided to approach problem from different angle and restrict amount of transactions user can have pending in the queue.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3088 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Single user can't flood transaction queue.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
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
        Created At 2023-06-05 09:43:28 +0000 UTC
    </div>
</div>

