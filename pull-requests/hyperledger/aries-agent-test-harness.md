---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/572" class=".btn">#572</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump json-schema and jsprim in /aries-backchannels/verity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [json-schema](https://github.com/kriszyp/json-schema) and [jsprim](https://github.com/joyent/node-jsprim). These dependencies needed to be updated together.
Updates `json-schema` from 0.2.3 to 0.4.0
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kriszyp/json-schema/commit/f6f6a3b02d667aa4ba2d5d50cc19208c4462abfa"><code>f6f6a3b</code></a> Use a little more robust method of checking instances</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/ef60987a9a14b9d9c739384460044ba53cd9b9a2"><code>ef60987</code></a> Update version</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/b62f1da1ff5442f23443d6be6a92d00e65cba93a"><code>b62f1da</code></a> Protect against constructor modification, <a href="https://github-redirect.dependabot.com/kriszyp/json-schema/issues/84">#84</a></li>
<li><a href="https://github.com/kriszyp/json-schema/commit/fb427cd4d175684786e4b2538718e72453e825e9"><code>fb427cd</code></a> Link to json-schema-org repository in addition to site, fixes <a href="https://github-redirect.dependabot.com/kriszyp/json-schema/issues/54">#54</a></li>
<li><a href="https://github.com/kriszyp/json-schema/commit/22f146111f541d9737e832823699ad3528ca7741"><code>22f1461</code></a> Don't allow <strong>proto</strong> property to be used for schema default/coerce, fixes <a href="https://github-redirect.dependabot.com/kriszyp/json-schema/issues/84">#84</a></li>
<li><a href="https://github.com/kriszyp/json-schema/commit/c52a27c653428149e4f9fb776d5e110d04639a9c"><code>c52a27c</code></a> Get basic test to pass</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/b3f42b3331608fe83b6cc267c5fc513ec1b839ed"><code>b3f42b3</code></a> Add security policy</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/3b0cec3042a5aac5c967fd43475f5edc4c5b6eff"><code>3b0cec3</code></a> Update version</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/c28470f2d64bace29c73d140f9c6876e3c3a9fef"><code>c28470f</code></a> Update readme to acknowledge the state of the package</li>
<li><a href="https://github.com/kriszyp/json-schema/commit/7dff9cd2c35c31ff3c43fa4e38737c94283dd3d3"><code>7dff9cd</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/kriszyp/json-schema/issues/81">#81</a> from hodovani/patch-1</li>
<li>Additional commits viewable in <a href="https://github.com/kriszyp/json-schema/compare/v0.2.3...v0.4.0">compare view</a></li>
</ul>
</details>
<br />

Updates `jsprim` from 1.4.1 to 1.4.2
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/TritonDataCenter/node-jsprim/blob/v1.4.2/CHANGES.md">jsprim's changelog</a>.</em></p>
<blockquote>
<h2>v1.4.2 (2021-11-29)</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/joyent/node-jsprim/issues/35">#35</a> Backport json-schema 0.4.0 to version 1.4.x</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/TritonDataCenter/node-jsprim/commit/5c8475fd44567e459b1b73b82f2669c39a0642b8"><code>5c8475f</code></a> <a href="https://github-redirect.dependabot.com/joyent/node-jsprim/issues/35">joyent/node-jsprim#35</a> Backport json-schema 0.4.0 to version 1.4.x</li>
<li>See full diff in <a href="https://github.com/joyent/node-jsprim/compare/v1.4.1...v1.4.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~bahamat">bahamat</a>, a new releaser for jsprim since your current version.</p>
</details>
<br />


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
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-agent-test-harness/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-05 14:34:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    Add ability to run the test scope of a runset normally executed daily by GitHub Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

A command that given the name of a runset (e.g. the tests run each night by GitHub Actions), grabs from that "workflow" YAML file the combination of agents used and the test scope, and then runs those.  Makes it easy to try out a runset to see where it is failing on your local system.  

Optionally allows you to do a `build` or `rebuild` before running the tests, and allows for doing a "dry-run" to printout what would be run.

Run `./manage runset -h` to get full help information and the list of runsets available.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-02 21:53:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Update aries-vcx backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates aries-vcx to the latest version, enables AFJ - aries-vcx tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 15:36:17 +0000 UTC
    </div>
</div>

