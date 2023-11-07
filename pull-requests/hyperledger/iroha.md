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
                PR <a href="https://github.com/hyperledger/iroha/pull/4033" class=".btn">#4033</a>
            </td>
            <td>
                <b>
                    [documentation]: Fixes the pytests README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                ## Description

Fixes the pytests README

### Linked issue

None

### Benefits

Correct README

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

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 14:41:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4032" class=".btn">#4032</a>
            </td>
            <td>
                <b>
                    [Documentation] Update message AddAssetQuantity and SubtractAssetQuantity with extra optional parameter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span><span class="chip">Documentation</span><span class="chip">api-changes</span>
            </td>
            <td>
                Add an optional argument title to AddAssetQuantity and SubtractAssetQuantity in commands.proto bufs. Make the C++ Iroha base core code handle it, make it working work. Improve the Gtests regarding to that change. Improve the Python client to handle that changes (provided in a separate repository).

Link to C++ library:
https://github.com/hyperledger/iroha/pull/4003/files

Link to Python client library which use protobuf GRPC shared code base:
https://github.com/hyperledger/iroha-python/

This is part of internship project:
https://wiki.hyperledger.org/display/INTERN/Iroha+1%3A+extend+queries+with+optional+arguments

Link to PR in iroha-python compatible with those changes:
hyperledger/iroha-python#157
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 09:01:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4031" class=".btn">#4031</a>
            </td>
            <td>
                <b>
                    [feature] #3974: Add subcommand into `iroha_client_cli` to transfer domains
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This pull request adds command to transfer domains between accounts into `iroha_client_cli`.

### Linked issue

Closes one of subtasks from #3974  

### Benefits

Extends the functionality of `iroha_client_cli`.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
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
        Created At 2023-11-03 08:59:54 +0000 UTC
    </div>
</div>

