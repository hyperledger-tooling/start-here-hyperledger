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
- **`iroha_swarm`:** now it relies on that `genesis.file` is written in the configuration file and is located under the `--config-dir`
- **`kagami`:** `kagami config peer` now accepts an optional argument `--genesis-file-in-config <PATH>` to set `genesis.file` in the output. Semantic analogous to `kagami genesis --executor-path-in-genesis <PATH>`.

### Linked issues

Closes #4029 #4105, partially addresses #4136

### Benefits

- Improves UX of configuration & usage of `iroha` and `iroha_client_cli`
- Moves more configuration responsibility to `iroha_config`
- Reduces complexity of init logic a little
### Checklist

- [ ] Technical writers review on CLIs
- [ ] https://github.com/hyperledger/iroha/pull/4139
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 00:15:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4149" class=".btn">#4149</a>
            </td>
            <td>
                <b>
                    [refactor]: Export iroha_crypto through iroha_client
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
        Created At 2023-12-13 12:27:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4148" class=".btn">#4148</a>
            </td>
            <td>
                <b>
                    [ci]: Use default settings for Coveralls action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

Use default settings for Coveralls action

### Linked issue
#4131 

### Benefits

Fix tests coverage should be compared against the iroha2-dev branch, not iroha2-stable.

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
        Created At 2023-12-13 12:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4147" class=".btn">#4147</a>
            </td>
            <td>
                <b>
                    [refactor]: Export iroha_config through iroha_client
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
        Created At 2023-12-13 12:09:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4146" class=".btn">#4146</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4080: Export iroha_data_model, iroha_config, iroha_crypto through iroha_client (#4081)
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
        Created At 2023-12-13 11:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4144" class=".btn">#4144</a>
            </td>
            <td>
                <b>
                    [feature]: add batching to `handle_pending_transactions`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description
The only thing in question is the fetch_size if either `vec.len() == 0` or `FetchSize.fetch_size.is_none()`

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4091 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

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
        Created At 2023-12-13 09:06:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4143" class=".btn">#4143</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4140: Fix registration of new peer
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
        Created At 2023-12-13 04:47:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4142" class=".btn">#4142</a>
            </td>
            <td>
                <b>
                    [fix] #4140: Fix registration of new peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

* Fixed new peer registration
* Fixed peer restart

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4140

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
        Created At 2023-12-12 16:46:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4139" class=".btn">#4139</a>
            </td>
            <td>
                <b>
                    [refactor]: split `iroha_torii` from `iroha`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">Chore</span>
            </td>
            <td>
                ## Description

This PR splits Torii (web server functionality), located in the main CLI, into a separate `iroha_torii` crate.

The rationale is to make a step towards making the main CLI exclusively a binary. Currently `iroha` is a library as well, exposing functionality to run `Iroha` in tests. That includes Torii. Since Torii is quite self-contained, making it a separate crate seem to make sense.

A further step would be to move `Iroha` itself and `iroha::samples` out of the CLI, so that `test_network` doesn't depend on `iroha` anymore, and `iroha` might be exclusively a binary.

Additionally:

- fix `telemetry` feature flag. Torii code didn't compile if this feature was disabled.
- clean dependencies of `iroha` CLI

### Linked issue

Addresses #4136, but doesn't close it.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 11:38:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4138" class=".btn">#4138</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #0000: On-chain predictable iteration order
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
        Created At 2023-12-12 08:28:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4135" class=".btn">#4135</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4090 #3858: Fix having to pass IROHA_SKIP_WASM_CHECKS env variable with true
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

I deleted the need to pass the IROHA_SKIP_WASM_CHECKS while building with stable toolchain and added in CI

### Linked issue

Closes #4090 #3858 <!-- Replace with an actual number,  -->




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-11 06:38:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4130" class=".btn">#4130</a>
            </td>
            <td>
                <b>
                    [fix] #0000: On-chain predictable iteration order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

* replace all `HashMap`/`HashSet` in `iroha_core` with `IndexMap`/`IndexSet`
* add `HashMap`/`HashSet` to `dissallowed_types` 

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes [#3](https://app.zenhub.com/workspaces/iroha-v2-60ddb820813b9100181fc060/issues/zh/3)

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
        Created At 2023-12-08 08:38:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4129" class=".btn">#4129</a>
            </td>
            <td>
                <b>
                    [refactor]: apply most recent clippy suggestions
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
        Created At 2023-12-08 07:53:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4128" class=".btn">#4128</a>
            </td>
            <td>
                <b>
                    [BACKPORT] #4120: Do not use the `tungstenite` re-exported from `tokio_tungstenite`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Re-exported does not have the TLS fully functional if we only enable it on `tokio-tungstenite`, so a direct dependency is required

### Linked issue

Fixes #4120

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] make ci pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 07:44:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4127" class=".btn">#4127</a>
            </td>
            <td>
                <b>
                    [documentation]: remove auto-generated configuration reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Documentation</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

This PR removes auto-generated configuration reference and everything related to it.

The motivation is to make one step forward towards the new reference (https://github.com/hyperledger/iroha-2-docs/issues/392). 

After merge of this PR, there will be no configuration reference available for some time. We decided that it is fine and will streamline further process according to the RFC (https://github.com/hyperledger/iroha/issues/2585).

Should be reviewed and merged after:

- #4100 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 07:04:51 +0000 UTC
    </div>
</div>

