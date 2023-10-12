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
                PR <a href="https://github.com/hyperledger/iroha/pull/3983" class=".btn">#3983</a>
            </td>
            <td>
                <b>
                    [feature] #3964: `application/x-parity-scale` response for `/status` …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

New features:

- `GET /status` accepts `application/x-parity-scale` content type and responds accordingly
- `GET /status/<field>` now accepts nested paths, e.g. `/status/uptime/secs`

__Breaking changes:__

- `GET /status/<field>` used to be forgiving for path-not-found and serialization errors. Now it returns 404 and 500 errors accordingly.

### Linked issue

Closes #3964

### Benefits

JavaScript SDK can use `/status` endpoint without hacks around JSON parsing.

### Checklist

- [x] Open a PR into documentation
  - https://github.com/hyperledger/iroha-2-docs/pull/422
- [x] Manually check the behaviour of `/status` endpoint
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-12 03:47:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3981" class=".btn">#3981</a>
            </td>
            <td>
                <b>
                    [refactor]: bump dependencies
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
        Created At 2023-10-11 13:06:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3980" class=".btn">#3980</a>
            </td>
            <td>
                <b>
                    [fix] #3971: Consensus bug fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Several bug fixes for sumeragi.

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3971 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 13:23:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3979" class=".btn">#3979</a>
            </td>
            <td>
                <b>
                    [refactor] #3874: Remove `IsAssetDefinitionOwner`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Notes
Two previous pull requests for the issue were closed without merge because of conflicts and messy commit histories. See #3919 #3920 . I have followed all the discussed steps in #3920 but some tests (in `mod.rs`) are still failing.


### Linked issue

This query was introduced only for the purposes of validator. Since #3442 we can use `FindAssetDefinitionById` to do the exact same thing.

Closes #3874 

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
        Created At 2023-10-10 11:57:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3977" class=".btn">#3977</a>
            </td>
            <td>
                <b>
                    Repairing MacOs build on develop
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span><span class="chip">1.5</span>
            </td>
            <td>
                ## Description
develop -> master is failing to compile in MacOs: https://github.com/hyperledger/iroha/pull/3960

That is why I need to repair the compilation.

I don't know if the commit will repair the problem:).

We need to wait
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
        Created At 2023-10-09 16:37:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3976" class=".btn">#3976</a>
            </td>
            <td>
                <b>
                    [refactor] #3918: Rename validator to executor
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

Closes #3918

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
        Created At 2023-10-09 13:02:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3973" class=".btn">#3973</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #3953: Add `owned_by` field to `Domain`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- Fixed unreachable isi
- Add `owned_by` to `Domain` and related permissions
- New tests

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3953, #3931, #3932 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Implement required feature, new tests, fixed bugs.

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
        Created At 2023-10-09 09:16:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3969" class=".btn">#3969</a>
            </td>
            <td>
                <b>
                    [ci] #3889: prune docker-compose files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Currently each branch (`iroha2-<lts|stable|dev>`) has set of docker-compose files not only for itself, but for other branches too. It leads to confusion and goes against how versioning works. Moreover, since `2.0` release will be relatively soon and we are going to get rid of channels at all, there is no sense to keep them in the dev branch.

This PR removes docker-compose files related to other branches/channels, and removes `.dev` suffix from the configurations related to `dev` branch.

### Linked issue

Closes #3889 (will be completely closed after merging into `iroha2-stable`)

### Benefits

Less confusion, natural branch-based versioning and CI checks

### Checklist

- [ ] Add CI check to ensure usage of a proper Dockerhub image according to the branch



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 02:58:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3968" class=".btn">#3968</a>
            </td>
            <td>
                <b>
                    [docs]: Remove `api_spec.md`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

The PR with API Reference in the documentation is merged:

- https://github.com/hyperledger/iroha-2-docs/pull/417

This PR removes the original, obsolete `api_spec.md` and sanitizes all references into it.

I also made some tech writing chores.

### Linked issue

_None_

### Checklist

- [ ] DevOps check
- [ ] Tech writers check of phrasing I used

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 02:20:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3967" class=".btn">#3967</a>
            </td>
            <td>
                <b>
                    [fix] proper rustc in devShell
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Small tweak to fix `rustc` in `devShell` not finding sysroot.

### Linked issue

None

### Benefits

Usable `rustc` in `devShell`

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
        Created At 2023-10-06 17:10:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3965" class=".btn">#3965</a>
            </td>
            <td>
                <b>
                     [fix] #3516: make FindTrigger queries return original WASM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Retain original WASM blobs in `TriggerSet`
Substitute internal representation for original when querying for Triggers
Remove internal representation from data_model

### Linked issue

Closes https://github.com/hyperledger/iroha/issues/3516

### Benefits

No more leaking internal representation
FindTrigger queries return actually useful WASM

### Checklist

- [ x] I've read `CONTRIBUTING.md`
- [ x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 01:04:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3963" class=".btn">#3963</a>
            </td>
            <td>
                <b>
                    [feature] #3953: Add `owned_by` field to `Domain`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- Fixed unreachable isi
- Add `owned_by` to `Domain` and related permissions
- New tests

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3953, #3931, #3932 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Implement required feature, new tests, fixed bugs.

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
        Created At 2023-10-05 14:55:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3960" class=".btn">#3960</a>
            </td>
            <td>
                <b>
                    Merge Iroha1 `develop` into `main`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span>
            </td>
            <td>
                There are several commits to be added.

----

removed duplicate code in goSrc/srcvmCaller/iroha/commands.go: 478

Signed-off-by: Sudhanshu <76694373+sudhanshu-k@users.noreply.github.com>## Description

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
        Created At 2023-10-05 09:12:56 +0000 UTC
    </div>
</div>

