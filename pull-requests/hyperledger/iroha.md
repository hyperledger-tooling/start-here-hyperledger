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
                PR <a href="https://github.com/hyperledger/iroha/pull/3549" class=".btn">#3549</a>
            </td>
            <td>
                <b>
                    [fix] #3548: Fix IntoSchema transparent attribute
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

- Fixed #[schema(transparent)]` for structs
- Added transparent type inference

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

- Closes #3548  <!-- Replace with an actual number,  -->

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
        Created At 2023-05-31 12:53:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3547" class=".btn">#3547</a>
            </td>
            <td>
                <b>
                    [fix] #3350: Core testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

This PR adds five new tests for sumeragi inside the core trait. I still need to refactor the PR to eliminate the duplicated code between the tests.


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
        Created At 2023-05-30 19:47:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3541" class=".btn">#3541</a>
            </td>
            <td>
                <b>
                    [fix] #3461: Logic error in defaults handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Make config params not specified in env or config file fall back to defaults. 

### Linked issue

Helps #3461. 

### Benefits

Less tedium

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 08:55:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3538" class=".btn">#3538</a>
            </td>
            <td>
                <b>
                    [fix] #3075: Panic on invalid tx in genesis.
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

Closes https://github.com/hyperledger/iroha/issues/3075

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
        Created At 2023-05-29 11:52:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3537" class=".btn">#3537</a>
            </td>
            <td>
                <b>
                    [ci]: Bump to RC16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Version bump to RC16 + push tags

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 08:11:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3536" class=".btn">#3536</a>
            </td>
            <td>
                <b>
                    [documentation] Changed the URL to install docker under prerequisites in the quick start guide section
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Changed the URL to install docker under prerequisites in the quick start guide section

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
        Created At 2023-05-26 12:37:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3534" class=".btn">#3534</a>
            </td>
            <td>
                <b>
                    [feature] #3533: Rename `Bool` to `bool` in schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Although it's inconsistent, sdk wants it this way

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #3533

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
        Created At 2023-05-26 07:12:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3532" class=".btn">#3532</a>
            </td>
            <td>
                <b>
                    Spelling Mistake
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
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
        Created At 2023-05-26 06:01:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/3531" class=".btn">#3531</a>
            </td>
            <td>
                <b>
                    Bump tornado from 5.1 to 6.3.2 in /docs/source
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [tornado](https://github.com/tornadoweb/tornado) from 5.1 to 6.3.2.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tornadoweb/tornado/blob/master/docs/releases.rst">tornado's changelog</a>.</em></p>
<blockquote>
<h1>Release notes</h1>
<p>.. toctree::
:maxdepth: 2</p>
<p>releases/v6.3.2
releases/v6.3.1
releases/v6.3.0
releases/v6.2.0
releases/v6.1.0
releases/v6.0.4
releases/v6.0.3
releases/v6.0.2
releases/v6.0.1
releases/v6.0.0
releases/v5.1.1
releases/v5.1.0
releases/v5.0.2
releases/v5.0.1
releases/v5.0.0
releases/v4.5.3
releases/v4.5.2
releases/v4.5.1
releases/v4.5.0
releases/v4.4.3
releases/v4.4.2
releases/v4.4.1
releases/v4.4.0
releases/v4.3.0
releases/v4.2.1
releases/v4.2.0
releases/v4.1.0
releases/v4.0.2
releases/v4.0.1
releases/v4.0.0
releases/v3.2.2
releases/v3.2.1
releases/v3.2.0
releases/v3.1.1
releases/v3.1.0
releases/v3.0.2
releases/v3.0.1
releases/v3.0.0
releases/v2.4.1
releases/v2.4.0
releases/v2.3.0
releases/v2.2.1
releases/v2.2.0
releases/v2.1.1</p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tornadoweb/tornado/commit/34f5c1cf2696afec5532ca9e870ba32cbc7fee27"><code>34f5c1c</code></a> Version 6.3.2</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/32ad07c54e607839273b4e1819c347f5c8976b2f"><code>32ad07c</code></a> web: Fix an open redirect in StaticFileHandler</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/e0fa53ee96db720dc7800d0248c39a4ffb8911e9"><code>e0fa53e</code></a> Merge pull request <a href="https://redirect.github.com/tornadoweb/tornado/issues/3257">#3257</a> from bdarnell/build-workflow-wstest-warning</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/f5a1d5c7e235ad8860a4c2c5f259a43692bcbaab"><code>f5a1d5c</code></a> ci: Only run pypi actions from the main repo</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/1849ef6c48415ef8f5fecbd47d9f68225588507c"><code>1849ef6</code></a> test: Close a websocket client that causes occasional test failures</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/fcb09eba4bd45c2ebfb6356a38acdb3b4450c0d8"><code>fcb09eb</code></a> Merge pull request <a href="https://redirect.github.com/tornadoweb/tornado/issues/3256">#3256</a> from bdarnell/build-workflow-qemu</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/c3d50f41a29cda5f76031c60cf7902b175b79479"><code>c3d50f4</code></a> ci: Update setup-qemu-action version</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/419838b9bcc51445241630def0478f1fbaa61b4b"><code>419838b</code></a> Merge pull request <a href="https://redirect.github.com/tornadoweb/tornado/issues/3255">#3255</a> from bdarnell/bump-version-6.3.1</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/cd5b9fcf4ac16c3f5480b3d8ae81b4103c0e7549"><code>cd5b9fc</code></a> Bump version to 6.3.1</li>
<li><a href="https://github.com/tornadoweb/tornado/commit/245334401570a40ba01813d9adb14976c50d77dd"><code>2453344</code></a> Merge pull request <a href="https://redirect.github.com/tornadoweb/tornado/issues/3254">#3254</a> from bdarnell/fix-set-cookie-case</li>
<li>Additional commits viewable in <a href="https://github.com/tornadoweb/tornado/compare/v5.1.0...v6.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tornado&package-manager=pip&previous-version=5.1&new-version=6.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2023-05-25 17:20:07 +0000 UTC
    </div>
</div>

