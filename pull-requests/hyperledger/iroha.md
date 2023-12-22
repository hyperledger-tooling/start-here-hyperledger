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
                PR <a href="https://github.com/hyperledger/iroha/pull/4165" class=".btn">#4165</a>
            </td>
            <td>
                <b>
                    [fix] #4164: Fix topology update on restart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Update current topology with block view change index.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4164 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Peer restarts correctly.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### How to test 

Use block store with where blocks have view change index > 0 and try to restart peer.

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
        Created At 2023-12-21 14:29:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4163" class=".btn">#4163</a>
            </td>
            <td>
                <b>
                    [feature] #3453: Implement Store CRUD Operations in Client CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

I added extra subcommands to asset which are set-store, get-store, remove-store, update-store

## Use Casees
```bash
./iroha_client_cli asset set-store --key="K4" --asset-id="tea##mad_hatter@looking_glass" --json --value="{ \"Vec\": [{\"String\": \"a\"}, {\"String\": \"b\"}] }"
---
./iroha_client_cli asset set-store --key="K4" --asset-id="tea##mad_hatter@looking_glass" --value=true
---
./iroha_client_cli asset update-store --key="K4" --asset-id="tea##mad_hatter@looking_glass" --value=16_u32
---
./iroha_client_cli asset get-store --key="K2" --asset-id="tea##mad_hatter@looking_glass"
---
./iroha_client_cli asset remove-store --key="K4" --asset-id="tea##mad_hatter@looking_glass"

```

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3453

<!-- Link if e.g. JIRA issue or  from another repository -->

### Checklist

- [ X] I've read `CONTRIBUTING.md`
- [ X] I've used the standard signed-off commit format (or will squash just before merging)
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
        Created At 2023-12-21 07:30:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4160" class=".btn">#4160</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4133: Count identical wasm for triggers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                - See also #4159 

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #4133 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

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
        Created At 2023-12-19 11:27:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4159" class=".btn">#4159</a>
            </td>
            <td>
                <b>
                    [fix] #4133: Count identical wasm for triggers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                - See also #4160

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #4133 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

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
        Created At 2023-12-19 11:26:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4157" class=".btn">#4157</a>
            </td>
            <td>
                <b>
                    [documentation]: update Pytests README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span>
            </td>
            <td>
                ## Description

Updated README (and `.gitignore`) in pytests because I found it confusing.

### Checklist

- [ ] Tech writers review
- [x] @AlexStroke review

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-18 04:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4156" class=".btn">#4156</a>
            </td>
            <td>
                <b>
                    [fix] #3857: Unify permission tokens in executor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Add unification of permission tokens in executor when granting permission tokens or registering role.
Unification is serialization and deserialization of permission token to remove ambiguity introduced by json format. 

I've tried approach proposed by original issue initially, but it didn't work well because:
- host in any case unable to check that permission tokens are indeed unified
- bloats amount of code
- it's still required to implement `Eq, Hash, ...` on `UnverifiedPermissionToken` because it's part of value

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3857 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Avoid certain bugs depending on permission token compassion. 

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
        Created At 2023-12-15 11:40:45 +0000 UTC
    </div>
</div>

