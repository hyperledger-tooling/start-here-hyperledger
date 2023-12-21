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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4153" class=".btn">#4153</a>
            </td>
            <td>
                <b>
                    [refactor] #4029, #4105, #4136: refactor CLIs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span><span class="chip">api-changes</span><span class="chip">config-changes</span><span class="chip">Refactor</span><span class="chip">UI</span>
            </td>
            <td>
                ## Description

**Changes:**

- **`iroha_genesis`:**
    - Refactor `GenesisNetwork` initialisation, remove side effects and simplify logic
    - Make `transactions` in `GenesisNetwork` non-public, to avoid invariant violation
- **`iroha_config`:**
    - Update Genesis config: instead of `account_public_key` and `account_private_key`, it now has `public_key`, `private_key`, and `file` options (according to #4029). Move some validation logic here (in form of `ParsedConfiguration` struct).
    - Finally, make `disable_panic_terminal_colors` deprecated option truly optional (#3506)
    - Use `PathBuf`s for all path parameters (`genesis.file`, `kura.block_store_path`, `snapshot.dir_path`, `telemetry.file`)
    - Update `Path` (multiple extensions support) behaviour
- **`iroha`:**
    - Use `clap`
    - Update CLI itself: `--config` argument, `--terminal-colors` (or `--terminal-colors=false`). `--submit-genesis` remains as is.
    - Update configuration pipeline:
        - Steps: defaults → file → env → build → validate & parse
        - If file is not specified, Iroha tries both `config.json` and `config.json5` and doesn't fail if they are not find (same as before)
        - If file is user-provided (`--config`, `IROHA_CONFIG=`) and it is not found, Iroha fails (previously it didn't)
        - _Read and parse_ ENV after file, not before
        - Resolve paths in the config file relatively to its location
- **`iroha_client_cli`:**
    - Update `clap` to `v4`, as in the rest of workspace
    - Refactor `--metadata` argument
    - Adopt the same configuration pipeline as in `iroha`
- **`iroha_swarm`:** explicitly specifies `config.json` and `genesis.json` paths in the generated docker-compose configurations
- **`kagami`:** `kagami config peer` now accepts an optional argument `--genesis-file-in-config <PATH>` to set `genesis.file` in the output. Semantic analogous to `kagami genesis --executor-path-in-genesis <PATH>`.

### Linked issues

Closes #4029 #4105, partially addresses #4136

### Benefits

- Improves UX of configuration & usage of `iroha` and `iroha_client_cli`
- Moves more configuration responsibility to `iroha_config`
- Reduces complexity of init logic a little

### Checklist

- [ ] Technical writers review on CLIs
- [x] https://github.com/hyperledger/iroha/pull/4139
- [x] Check docker compose files manually
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 00:15:45 +0000 UTC
    </div>
</div>

