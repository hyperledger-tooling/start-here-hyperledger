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
                PR <a href="https://github.com/hyperledger/iroha/pull/3790" class=".btn">#3790</a>
            </td>
            <td>
                <b>
                    [ci]: Fix I2:Release  job & Remove badge and load-rs job & Update i2 …
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                [ci]: Update iroha2 `I2::Dev::Publish` and `I2::Release::Publish` workflows.

## Description
1. Fix I2:Release `configs` job.
2. Remove `coveralls` badge (it works only on the default repository branch).
3. Remove `load-rs` CI dispatch trigger workflow (there is no need to trigger load-rs script build anymore).
4. Fix iroha2 user rootless `GID` inside i2 Alpine image.
5. Modify iroha2:stable and iroha2:lts images tags. Now it will be `iroha2:stable-2.0.0-pre-rc.18` or  `iroha2:lts-2.0.0-pre-rc.19`tags. I think there is not a read need to add `${{ github.sha }}` there into tags names like `lts-${{ env.VERSION }}-${{ github.sha }}`.

### Linked issue
Covers #3430 and #3771 

### Benefits
Cover issues requests and improve iroha2 CI.

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
        Created At 2023-08-08 17:27:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3789" class=".btn">#3789</a>
            </td>
            <td>
                <b>
                    [feature] #2885: Add `NotificationEvent`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Added new type of event `NotificationEvent` and split event filters into 2 types which can be attached to trigger and which can't.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #2885 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

More detailed information about operation of iroha node.

### Drawbacks

Emitting events has non-zero cost.

I'm not entirely sure that splitting event filters into triggerable and ordinary once is wroth it (since it require some code duplication) + not sure why we should omit attaching trigger to notification events.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### How to test

* Run tests:

```bash
# run integration tests
cargo test --package iroha_client --test mod -- integration::events::notification --nocapture 

# run unit test for filter matching
cargo test --package iroha_data_model --features transparent_api --lib -- events::notification::tests::trigger_completed_events_filter --exact --nocapture
```

* On live iroha node:
1. Start iroha
2. Register some triggers

register_trigger_failbox.json
```json
[
    {
        "Register": {
            "Trigger": {
            "Raw": {
                "id": "fail_box",
                "action": {
                "executable": {
                    "Instructions": [
                    {
                        "Fail": "Error"
                    }
                    ]
                },
                "repeats": "Indefinitely",
                "authority": "alice@wonderland",
                "filter": {
                    "ExecuteTrigger": {
                    "trigger_id": "fail_box",
                    "authority": "alice@wonderland"
                    }
                },
                "metadata": {}
                }
            }
            }
        }
    }
]
```

register_trigger_mint.json
```
[
    {
        "Register": {
            "Trigger": {
            "Raw": {
                "id": "mint_rose",
                "action": {
                "executable": {
                    "Instructions": [
                    {
                        "Mint": {
                        "U32": 1,
                        "destination_id": {
                            "AssetId": "rose##alice@wonderland"
                        }
                        }
                    }
                    ]
                },
                "repeats": "Indefinitely",
                "authority": "alice@wonderland",
                "filter": {
                    "ExecuteTrigger": {
                    "trigger_id": "mint_rose",
                    "authority": "alice@wonderland"
                    }
                },
                "metadata": {}
                }
            }
            }
        }
    }
]
```

```bash
cat ./register_trigger_failbox.json | ./iroha_client_cli json
cat ./register_trigger_mint.json | ./iroha_client_cli json
```

3. Start listening for events 

```bash
./iroha_client_cli events notification
```

4. Trigger trigger execution

execute_trigger_failbox.json
```json
[
    {
        "ExecuteTrigger": {
            "TriggerId": "fail_box"
        }
    }
]
```

execute_trigger_mint.json
```json
[
    {
        "ExecuteTrigger": {
            "TriggerId": "mint_rose"
        }
    }
]
```

```bash
cat ./execute_trigger_failbox.json | ./iroha_client_cli json
cat ./execute_trigger_mint.json | ./iroha_client_cli json
```

5. Check command from step 3. for presence of events in the output

### Checklist

- [x] Add `NotificationEvent` and it's filter
- [x] Emit event after trigger complition
- [x] Add unit and integration tests to cover new functionality
- [x] Add `iroha_client_cli` support for new feature 

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
        Created At 2023-08-08 11:33:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3788" class=".btn">#3788</a>
            </td>
            <td>
                <b>
                    [fix] #2245: Nix build iroha node binary as AppImage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

I have found an AppImage bundler for nix and converted it for use in our nix flake. You can now run `nix build .#appimage` to build the iroha node binary as an AppImage. Ideally we would build all the projects binaries but for now that was outside of my skills with nix.

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Partially closes #2245  <!-- Replace with an actual number,  -->

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
        Created At 2023-08-08 07:26:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3785" class=".btn">#3785</a>
            </td>
            <td>
                <b>
                    [feature] #3780: Add tini to forward signals to processes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Add [Tini](https://github.com/krallin/tini) to pass signals to the Iroha processes.
Sets up Tini using its current builds, and uses GPG for the certificate checks.
**GPG build part unchecked; this is a draft.**

Modifies Dockerfiles:

* https://github.com/hyperledger/iroha/blob/iroha2-dev/Dockerfile
* https://github.com/hyperledger/iroha/blob/iroha2-dev/Dockerfile.build

* https://github.com/hyperledger/iroha/blob/iroha2-dev/Dockerfile.glibc
* https://github.com/hyperledger/iroha/blob/iroha2-dev/Dockerfile.build.glibc

### Linked issue

https://github.com/hyperledger/iroha/issues/3780

### Benefits

The Iroha processes will shut down normally.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-08 06:23:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3784" class=".btn">#3784</a>
            </td>
            <td>
                <b>
                    [feature] #3781: Validate genesis transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">Executor</span>
            </td>
            <td>
                ## Description

- Added new parameter `block_height` for all Validator entrypoints
- `block_height` can also be achieved from Smartcontracts and Triggers but it's not mandatory in entrypoint signature
- Implemented real genesis validation on Iroha side
- Added test

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3781 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Genesis Permission Tokens validation
- Validator will get **all** transactions, which it may want to be able to configure its state somehow

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
        Created At 2023-08-07 19:22:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3782" class=".btn">#3782</a>
            </td>
            <td>
                <b>
                    [feature] #3324: Add client cli burn checks and refactoring
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

Closes #3324 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

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
        Created At 2023-08-04 10:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3778" class=".btn">#3778</a>
            </td>
            <td>
                <b>
                    [fix] #3777: Validate role registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

- Default Validator now returns error if decoding failed instead of a panic
- Added role registration validation
- Added test which ensures that role with invalid tokens won't be registered.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3777 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

- Validator won't panic on decoding error
- Invalid roles won't pass registration

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
        Created At 2023-08-03 16:14:34 +0000 UTC
    </div>
</div>

