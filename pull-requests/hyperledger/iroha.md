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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4122" class=".btn">#4122</a>
            </td>
            <td>
                <b>
                    [fix] #4120: Do not use the `tungstenite` re-exported from `tokio_tungstenite`
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

### Checklist

- [x] make ci pass

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 15:48:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4118" class=".btn">#4118</a>
            </td>
            <td>
                <b>
                    [refactor]: update `iroha_cli_derive` to use syn 2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description
A part of #3682

Seems like we do not need to introduce manyhow and darling for this crate

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4117 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
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
        Created At 2023-12-07 04:38:34 +0000 UTC
    </div>
</div>

