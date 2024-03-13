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
                PR <a href="https://github.com/hyperledger/iroha/pull/4365" class=".btn">#4365</a>
            </td>
            <td>
                <b>
                    [feature] #4059: snapshots "mode"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

- Introduce `mode` of snapshots behaviour: `normal` (read & write), `readonly`, and `disabled`
- Run `SnapshotMaker` actor only in `normal` mode
- Configuration: remove `snapshot.creation_enabled`, add `snapshot.mode`
- Recursively create directories on snapshot writing (#4296)
- Update related logging
- Add tests

### Linked issue

Closes #4059, #4296 

### Benefits

More expected behaviour of snapshots for users?


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-13 10:17:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4357" class=".btn">#4357</a>
            </td>
            <td>
                <b>
                    [refactor] #3682: Remove all direct dependencies on syn 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

This concludes the syn 2 migration saga, removing all mentions of it from the codebase. It also removes the `syn2` renaming of the new version, as we are no longer depending on two versions at the same time. 

We still have syn 1 as a transitive dependency on syn 1 though =(

I suggest reviewing the two commits separately, as the blank rename of `syn2` to `syn` is very noisy

### Linked issue

Closes #3682

### Benefit

Less complexity due to use of multiple versions of the same library; only the shiny new API.

### Checklist

- [ ] make CI pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 12:36:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4349" class=".btn">#4349</a>
            </td>
            <td>
                <b>
                    [feature] #4244: Allow granting/revoking role's permissions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

Allow granting/revoking permissions from roles.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4244 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Roles are more flexible.

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
        Created At 2024-03-06 13:08:52 +0000 UTC
    </div>
</div>

