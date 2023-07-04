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
                PR <a href="https://github.com/hyperledger/iroha/pull/3678" class=".btn">#3678</a>
            </td>
            <td>
                <b>
                    [chore]: add @DCNick3 to the CODEOWNERS
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
        Created At 2023-07-04 14:09:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3676" class=".btn">#3676</a>
            </td>
            <td>
                <b>
                    [ci]: update dependabot
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
        Created At 2023-07-04 12:28:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3675" class=".btn">#3675</a>
            </td>
            <td>
                <b>
                    [feature] #3383: Implement a macro that parses a socket address at compile time
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Linked issue

Closes #3383 

### Limitations

This can't replace all uses of the existing `socket_addr!` macro, as it parses only literal addresses. Some of the `socket_addr!` usages use an expression as port number: https://github.com/hyperledger/iroha/blob/19984d91c2add850a197050e6cbee52af1bc6fa2/core/test_network/src/lib.rs#L598. Supporting this is possible, but would require a more complicated parser.

As 5/11 usages of the original macro use it, it probably doesn't make sense to merge it without support for variable ports

It also doesn't support hostname addresses, but they are not used anywhere except in the doc-test for the `socket_addr!` macro. Probably fine going without it, but should be relatively easy to implement if needed.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 11:52:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3669" class=".btn">#3669</a>
            </td>
            <td>
                <b>
                    [ci] #3648: include `docker-compose.*.yml` check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description

This PR adds a CI/CD check that `docker-compose.*.yml` files stored in the repo are generated with `kagami swarm` tool. This PR includes updated Docker Compose configurations as well.

### Linked issue

Closes #3648

### Benefits

It will help to be sure that those files are up-to-date, therefore to avoid confusion of any Iroha users.

### Checklist

- [ ] Ensure that the PR covers **all** Docker Compose files that should be covered.
- [ ] Discuss `docker-compose.TML.yml` in the `check.sh`
- [ ] Discuss/ensure that the check runs in the correct time, as described in #3648: selective run on changes in data model / kagami swarm code, etc
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-03 06:56:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3667" class=".btn">#3667</a>
            </td>
            <td>
                <b>
                    [refactor]: reject incorrect config topology early
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
        Created At 2023-07-01 19:29:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3666" class=".btn">#3666</a>
            </td>
            <td>
                <b>
                    [feature] #3665: remove max log query from wasm
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

Closes #3665

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
        Created At 2023-07-01 19:29:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3664" class=".btn">#3664</a>
            </td>
            <td>
                <b>
                    Bump pipreqs from 0.4.9 to 0.4.12 in /docs/source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pipreqs](https://github.com/bndr/pipreqs) from 0.4.9 to 0.4.12.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/bndr/pipreqs/releases">pipreqs's releases</a>.</em></p>
<blockquote>
<h2>v0.4.12</h2>
<p>I've noticed the PyPi package was not updated in a long time, so I created a new released with the latest changes from last 2 years or so.</p>
<p>Thank you everyone who contributed.</p>
<h2>What's Changed</h2>
<ul>
<li>Require Python 3.7 or higher by <a href="https://github.com/EwoutH"><code>@​EwoutH</code></a> in <a href="https://redirect.github.com/bndr/pipreqs/pull/339">bndr/pipreqs#339</a></li>
<li>resolve issue <a href="https://redirect.github.com/bndr/pipreqs/issues/285">#285</a> by <a href="https://github.com/clvnkhr"><code>@​clvnkhr</code></a> in <a href="https://redirect.github.com/bndr/pipreqs/pull/344">bndr/pipreqs#344</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/EwoutH"><code>@​EwoutH</code></a> made their first contribution in <a href="https://redirect.github.com/bndr/pipreqs/pull/339">bndr/pipreqs#339</a></li>
<li><a href="https://github.com/clvnkhr"><code>@​clvnkhr</code></a> made their first contribution in <a href="https://redirect.github.com/bndr/pipreqs/pull/344">bndr/pipreqs#344</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/bndr/pipreqs/compare/v0.4.10...v0.4.12">https://github.com/bndr/pipreqs/compare/v0.4.10...v0.4.12</a></p>
<h2>v0.4.11</h2>
<ul>
<li>added =&gt; and ~= support through the &quot;mode&quot; option</li>
<li>mapping updates, small bug fixes and increased test coverage</li>
</ul>
<h2>v0.4.10</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/bndr/pipreqs/blob/master/HISTORY.rst">pipreqs's changelog</a>.</em></p>
<blockquote>
<p>.. :changelog:</p>
<h2>History</h2>
<h2>0.4.11 (2020-03-29)</h2>
<ul>
<li>Implement '--mode' (Jake Teo, Jerome Chan)</li>
</ul>
<h2>0.4.8 (2017-06-30)</h2>
<ul>
<li>Implement '--clean' and '--diff' (kxrd)</li>
<li>Exclude concurrent{,.futures} from stdlib if py2 (kxrd)</li>
</ul>
<h2>0.4.7 (2017-04-20)</h2>
<ul>
<li>BUG: remove package/version duplicates</li>
<li>Style: pep8</li>
</ul>
<h2>0.4.5 (2016-12-13)</h2>
<ul>
<li>Fixed the --pypi-server option</li>
</ul>
<h2>0.4.4 (2016-07-14)</h2>
<ul>
<li>Remove Spaces in output</li>
<li>Add package to output even without version</li>
</ul>
<h2>0.4.2 (2016-02-10)</h2>
<ul>
<li>Fix duplicated lines in requirements.txt (Dmitry Pribysh)</li>
</ul>
<h2>0.4.1 (2016-02-05)</h2>
<ul>
<li>Added ignore option (Nick Rhinehart)</li>
</ul>
<h2>0.4.0 (2016-01-28)</h2>
<ul>
<li>Walk Abstract Syntax Tree to find imports (Kay Sackey)</li>
</ul>
<h2>0.3.9 (2016-01-20)</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/bndr/pipreqs/commits/v0.4.12">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pipreqs&package-manager=pip&previous-version=0.4.9&new-version=0.4.12)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/iroha/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-30 22:18:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3663" class=".btn">#3663</a>
            </td>
            <td>
                <b>
                    [feature] #3309: Bumps `wasmtime` version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

1. Replaces error lifting from `Trap` with `wasmtime::Error` that is `anyhow::Error` actually.
2. Replaces all codec errors with structured errors.
3. Replaces `eyre` with `wasmtime::Error` in structured errors related to executing smart-contracts.

### Linked issue

Closes #3309 

### Benefits

Upgrades `wasmtime` to the latest version.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
- [ ] Fix FFI troubles

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
        Created At 2023-06-30 16:36:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3661" class=".btn">#3661</a>
            </td>
            <td>
                <b>
                    [feature] #3236: Enhance iroha_wasm_builder with cache, better errors and minor API changes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Optimization</span>
            </td>
            <td>
                ## Description

Now you can configure `iroha_wasm_builder` output dir in a three ways (in order of priority):

1. Explicitly use `out_dir()` method
2. Set `IROHA_WASM_BUILDER_OUT_DIR` env var
3. Do nothing if you are in a build-script. Directory will be inherited from `OUT_DIR` env var which is set by `cargo`

By default `target` directory of running crate will be used.

Other than that optimization *caching* is also implemented.
This is done by comparing `sha256` hashes of non-omptimized wasm-files. If hash before and after build are equal, then non-omptimized file wasn't changed, which means that optimized wasm file should also stay unchanged and we don't have to spent time on running `wasm-opt`.

Also `build()` will fail now if it's being called on workspace. I think, it was an error that we didn't have that before. It's an error because we run `build()` only to get `Output` from it, where `Output` is a binary encoded WASM file, which we can't choose if we build workspace.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3236 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Cached wasm binaries allows us not to rebuild them everytime from scratch. I.e. cached validator builds now take much less time. Same for tests which sumbit wasm.

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
        Created At 2023-06-29 14:13:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3659" class=".btn">#3659</a>
            </td>
            <td>
                <b>
                    [fix] #3543: Increment quantity change, not total
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

Closes #3543


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 12:22:32 +0000 UTC
    </div>
</div>

