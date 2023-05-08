---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2417" class=".btn">#2417</a>
            </td>
            <td>
                <b>
                    feat(connector-tcs-huawei):  Initial commit of feature tcs-huawei connector.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                tcs-huawei and the blockchains connected to tcs-huawei can be integrated to cactus by this connector.

Signed-off-by: Wang Yinglun wangyinglun3@huawei.com 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 06:19:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2416" class=".btn">#2416</a>
            </td>
            <td>
                <b>
                    fix(vscode/devcontainer): unexpected exit stdout /etc/passwd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Moved away from trying to handroll an Ubuntu-22.04 image for the dev container
and instead used the "features" feature (no pun intended) of the dev container
spec: https://code.visualstudio.com/blogs/2022/09/15/dev-container-features
2. This produces a container that builds and launches reliably without the
issues the previous version was suffering from (which was that to some people
the container would just exit randomly during the launch)
3. Our future goal of having the dev container being built in a reproducible
way is still not achieved, but we've gotten closer because in the meantime
while working on this issue it was discovered that we can re-build the images
directly from the CLI by using the dev container CLI package:
https://github.com/devcontainers/cli
4. The upside of not building the image from scratch is that we can count on
future improvements/maintenance from others who are working on these images.
5. The downside of not building the image from scratch is that if we end up
finding something that does not work due to the customizations, it might be
more difficult to figure that out compared to if we had just build our own.
6. It is hard to predcit right now whether 4) or 5) will end up being having
the stronger effect, but we can cross that bridge when we get to it.
7. In the meantime I've started working on a contribution to the dev container
CLI itself for a dockerfile ejection feature (meaning that we'll be able to
render a single Dockerfile for the dev container (that right now the CLI only
stores/uses internally in it's own code at runtime). This eject feature will
be good for debugging purposes in case anything goes wrong with the image in the
future.

Fixes #2404

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 17:34:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2415" class=".btn">#2415</a>
            </td>
            <td>
                <b>
                    chore(ci): publish weaver go modules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Chore:
- chore(ci): publish weaver go modules
   This way of publishing all go modules in single commit will work as long as in the release commit, only version files are changed and script `go-gen-checksum.sh` in root directory is run, and no other changes are made between that commit and actual releasing (i.e. no other PR is merged affecting these go modules till release PR is merged).

Fixes:
- fix(ci): update version only if tag has version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 06:37:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2414" class=".btn">#2414</a>
            </td>
            <td>
                <b>
                    feat(openssl): version upgrade to v0.10.48 in cactus-plugin-keychain-vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix: issue #2365
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 10:58:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2413" class=".btn">#2413</a>
            </td>
            <td>
                <b>
                    chore(ci): enable weaver deployment workflows triggered on tag release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - chore(ci): enable weaver deployment workflows triggered on tag release (except go modules)
 - feat(ci): pre-release test if all weaver module versions are same
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-02 12:43:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2410" class=".btn">#2410</a>
            </td>
            <td>
                <b>
                    build(deps): bump flask from 2.0.1 to 2.3.2 in /packages-python/cactus_validator_socketio_indy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [flask](https://github.com/pallets/flask) from 2.0.1 to 2.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/flask/releases">flask's releases</a>.</em></p>
<blockquote>
<h2>2.3.2</h2>
<p>This is a security fix release for the 2.3.x release branch.</p>
<ul>
<li>Security advisory: <a href="https://github.com/pallets/flask/security/advisories/GHSA-m2qf-hxjv-5gpq">https://github.com/pallets/flask/security/advisories/GHSA-m2qf-hxjv-5gpq</a>, CVE-2023-30861</li>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-2">https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/29?closed=1">https://github.com/pallets/flask/milestone/29?closed=1</a></li>
</ul>
<h2>2.3.1</h2>
<p>This is a fix release for the 2.3.x release branch.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-1">https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/28?closed=1">https://github.com/pallets/flask/milestone/28?closed=1</a></li>
</ul>
<h2>2.3.0</h2>
<p>This is a feature release, which includes new features, removes previously deprecated code, and adds new deprecations. The 2.3.x branch is now the supported fix branch, the 2.2.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades. Test with warnings treated as errors to be able to adapt to deprecation warnings early.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-0">https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/24?closed=1">https://github.com/pallets/flask/milestone/24?closed=1</a></li>
</ul>
<h2>2.2.4</h2>
<p>This is a fix release for the 2.2.x release branch.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-4">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-4</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/27?closed=1">https://github.com/pallets/flask/milestone/27?closed=1</a></li>
</ul>
<h2>2.2.3</h2>
<p>This is a fix release for the 2.2.x release branch.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-3">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/26?closed=1">https://github.com/pallets/flask/milestone/26?closed=1</a></li>
</ul>
<h2>2.2.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/flask/releases/tag/2.2.0">2.2.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-2">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/25?closed=1">https://github.com/pallets/flask/milestone/25?closed=1</a></li>
</ul>
<h2>2.2.1</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/flask/releases/tag/2.2.0">2.2.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-1">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/23?closed=1">https://github.com/pallets/flask/milestone/23?closed=1</a></li>
</ul>
<h2>2.2.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated code. The 2.2.x branch is now the supported bug fix branch, the 2.1.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-0">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/19?closed=1">https://github.com/pallets/flask/milestone/19?closed=1</a></li>
</ul>
<h2>2.1.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/flask/blob/main/CHANGES.rst">flask's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.3.2</h2>
<p>Released 2023-05-01</p>
<ul>
<li>Set <code>Vary: Cookie</code> header when the session is accessed, modified, or refreshed.</li>
<li>Update Werkzeug requirement to &gt;=2.3.3 to apply recent bug fixes.</li>
</ul>
<h2>Version 2.3.1</h2>
<p>Released 2023-04-25</p>
<ul>
<li>Restore deprecated <code>from flask import Markup</code>. :issue:<code>5084</code></li>
</ul>
<h2>Version 2.3.0</h2>
<p>Released 2023-04-25</p>
<ul>
<li>
<p>Drop support for Python 3.7. :pr:<code>5072</code></p>
</li>
<li>
<p>Update minimum requirements to the latest versions: Werkzeug&gt;=2.3.0, Jinja2&gt;3.1.2,
itsdangerous&gt;=2.1.2, click&gt;=8.1.3.</p>
</li>
<li>
<p>Remove previously deprecated code. :pr:<code>4995</code></p>
<ul>
<li>The <code>push</code> and <code>pop</code> methods of the deprecated <code>_app_ctx_stack</code> and
<code>_request_ctx_stack</code> objects are removed. <code>top</code> still exists to give
extensions more time to update, but it will be removed.</li>
<li>The <code>FLASK_ENV</code> environment variable, <code>ENV</code> config key, and <code>app.env</code>
property are removed.</li>
<li>The <code>session_cookie_name</code>, <code>send_file_max_age_default</code>, <code>use_x_sendfile</code>,
<code>propagate_exceptions</code>, and <code>templates_auto_reload</code> properties on <code>app</code>
are removed.</li>
<li>The <code>JSON_AS_ASCII</code>, <code>JSON_SORT_KEYS</code>, <code>JSONIFY_MIMETYPE</code>, and
<code>JSONIFY_PRETTYPRINT_REGULAR</code> config keys are removed.</li>
<li>The <code>app.before_first_request</code> and <code>bp.before_app_first_request</code> decorators
are removed.</li>
<li><code>json_encoder</code> and <code>json_decoder</code> attributes on app and blueprint, and the
corresponding <code>json.JSONEncoder</code> and <code>JSONDecoder</code> classes, are removed.</li>
<li>The <code>json.htmlsafe_dumps</code> and <code>htmlsafe_dump</code> functions are removed.</li>
<li>Calling setup methods on blueprints after registration is an error instead of a
warning. :pr:<code>4997</code></li>
</ul>
</li>
<li>
<p>Importing <code>escape</code> and <code>Markup</code> from <code>flask</code> is deprecated. Import them
directly from <code>markupsafe</code> instead. :pr:<code>4996</code></p>
</li>
<li>
<p>The <code>app.got_first_request</code> property is deprecated. :pr:<code>4997</code></p>
</li>
<li>
<p>The <code>locked_cached_property</code> decorator is deprecated. Use a lock inside the
decorated function if locking is needed. :issue:<code>4993</code></p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/flask/commit/f3b8f570545200c87465d18386f3fc9f2258307a"><code>f3b8f57</code></a> release version 2.3.2</li>
<li><a href="https://github.com/pallets/flask/commit/c990bba94ab9bc81adf2d33e83c9a9628a2098f2"><code>c990bba</code></a> update min test env</li>
<li><a href="https://github.com/pallets/flask/commit/adedb2a64ea7703369bc89021710b439ee79f8dc"><code>adedb2a</code></a> Merge pull request <a href="https://redirect.github.com/pallets/flask/issues/5101">#5101</a> from pallets/update-werkzeug</li>
<li><a href="https://github.com/pallets/flask/commit/e1aedecdc689cc9a79131851dbdabf6c3bc49c9e"><code>e1aedec</code></a> update werkzeug</li>
<li><a href="https://github.com/pallets/flask/commit/37badc3ce8b0665e3454547839196a676729309f"><code>37badc3</code></a> update changelog</li>
<li><a href="https://github.com/pallets/flask/commit/70f906c51ce49c485f1d355703e9cc3386b1cc2b"><code>70f906c</code></a> Merge pull request from GHSA-m2qf-hxjv-5gpq</li>
<li><a href="https://github.com/pallets/flask/commit/8705dd39c4fa563ea0fe0bf84c85da8fcc98b88d"><code>8705dd3</code></a> set <code>Vary: Cookie</code> header consistently for session</li>
<li><a href="https://github.com/pallets/flask/commit/9532cba45d2339e90ebf04f178b1e4f2064e7328"><code>9532cba</code></a> fix mypy finding</li>
<li><a href="https://github.com/pallets/flask/commit/0bc7356ce1ae11e633426902aba76d525f4523da"><code>0bc7356</code></a> start version 2.3.2</li>
<li><a href="https://github.com/pallets/flask/commit/f07fb2b607c1eaa724ca9bfe43e2dc20d97d34de"><code>f07fb2b</code></a> Merge pull request <a href="https://redirect.github.com/pallets/flask/issues/5086">#5086</a> from pallets/release-2.3.1</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/flask/compare/2.0.1...2.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=flask&package-manager=pip&previous-version=2.0.1&new-version=2.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 23:12:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2409" class=".btn">#2409</a>
            </td>
            <td>
                <b>
                    build(deps): bump flask from 2.0.1 to 2.3.2 in /packages-python/cactus_validator_socketio_indy/validator-python
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [flask](https://github.com/pallets/flask) from 2.0.1 to 2.3.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/flask/releases">flask's releases</a>.</em></p>
<blockquote>
<h2>2.3.2</h2>
<p>This is a security fix release for the 2.3.x release branch.</p>
<ul>
<li>Security advisory: <a href="https://github.com/pallets/flask/security/advisories/GHSA-m2qf-hxjv-5gpq">https://github.com/pallets/flask/security/advisories/GHSA-m2qf-hxjv-5gpq</a>, CVE-2023-30861</li>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-2">https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/29?closed=1">https://github.com/pallets/flask/milestone/29?closed=1</a></li>
</ul>
<h2>2.3.1</h2>
<p>This is a fix release for the 2.3.x release branch.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-1">https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/28?closed=1">https://github.com/pallets/flask/milestone/28?closed=1</a></li>
</ul>
<h2>2.3.0</h2>
<p>This is a feature release, which includes new features, removes previously deprecated code, and adds new deprecations. The 2.3.x branch is now the supported fix branch, the 2.2.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades. Test with warnings treated as errors to be able to adapt to deprecation warnings early.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-0">https://flask.palletsprojects.com/en/2.3.x/changes/#version-2-3-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/24?closed=1">https://github.com/pallets/flask/milestone/24?closed=1</a></li>
</ul>
<h2>2.2.4</h2>
<p>This is a fix release for the 2.2.x release branch.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-4">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-4</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/27?closed=1">https://github.com/pallets/flask/milestone/27?closed=1</a></li>
</ul>
<h2>2.2.3</h2>
<p>This is a fix release for the 2.2.x release branch.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-3">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/26?closed=1">https://github.com/pallets/flask/milestone/26?closed=1</a></li>
</ul>
<h2>2.2.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/flask/releases/tag/2.2.0">2.2.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-2">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/25?closed=1">https://github.com/pallets/flask/milestone/25?closed=1</a></li>
</ul>
<h2>2.2.1</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/flask/releases/tag/2.2.0">2.2.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-1">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/23?closed=1">https://github.com/pallets/flask/milestone/23?closed=1</a></li>
</ul>
<h2>2.2.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated code. The 2.2.x branch is now the supported bug fix branch, the 2.1.x branch will become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades.</p>
<ul>
<li>Changes: <a href="https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-0">https://flask.palletsprojects.com/en/2.2.x/changes/#version-2-2-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/flask/milestone/19?closed=1">https://github.com/pallets/flask/milestone/19?closed=1</a></li>
</ul>
<h2>2.1.3</h2>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/flask/blob/main/CHANGES.rst">flask's changelog</a>.</em></p>
<blockquote>
<h2>Version 2.3.2</h2>
<p>Released 2023-05-01</p>
<ul>
<li>Set <code>Vary: Cookie</code> header when the session is accessed, modified, or refreshed.</li>
<li>Update Werkzeug requirement to &gt;=2.3.3 to apply recent bug fixes.</li>
</ul>
<h2>Version 2.3.1</h2>
<p>Released 2023-04-25</p>
<ul>
<li>Restore deprecated <code>from flask import Markup</code>. :issue:<code>5084</code></li>
</ul>
<h2>Version 2.3.0</h2>
<p>Released 2023-04-25</p>
<ul>
<li>
<p>Drop support for Python 3.7. :pr:<code>5072</code></p>
</li>
<li>
<p>Update minimum requirements to the latest versions: Werkzeug&gt;=2.3.0, Jinja2&gt;3.1.2,
itsdangerous&gt;=2.1.2, click&gt;=8.1.3.</p>
</li>
<li>
<p>Remove previously deprecated code. :pr:<code>4995</code></p>
<ul>
<li>The <code>push</code> and <code>pop</code> methods of the deprecated <code>_app_ctx_stack</code> and
<code>_request_ctx_stack</code> objects are removed. <code>top</code> still exists to give
extensions more time to update, but it will be removed.</li>
<li>The <code>FLASK_ENV</code> environment variable, <code>ENV</code> config key, and <code>app.env</code>
property are removed.</li>
<li>The <code>session_cookie_name</code>, <code>send_file_max_age_default</code>, <code>use_x_sendfile</code>,
<code>propagate_exceptions</code>, and <code>templates_auto_reload</code> properties on <code>app</code>
are removed.</li>
<li>The <code>JSON_AS_ASCII</code>, <code>JSON_SORT_KEYS</code>, <code>JSONIFY_MIMETYPE</code>, and
<code>JSONIFY_PRETTYPRINT_REGULAR</code> config keys are removed.</li>
<li>The <code>app.before_first_request</code> and <code>bp.before_app_first_request</code> decorators
are removed.</li>
<li><code>json_encoder</code> and <code>json_decoder</code> attributes on app and blueprint, and the
corresponding <code>json.JSONEncoder</code> and <code>JSONDecoder</code> classes, are removed.</li>
<li>The <code>json.htmlsafe_dumps</code> and <code>htmlsafe_dump</code> functions are removed.</li>
<li>Calling setup methods on blueprints after registration is an error instead of a
warning. :pr:<code>4997</code></li>
</ul>
</li>
<li>
<p>Importing <code>escape</code> and <code>Markup</code> from <code>flask</code> is deprecated. Import them
directly from <code>markupsafe</code> instead. :pr:<code>4996</code></p>
</li>
<li>
<p>The <code>app.got_first_request</code> property is deprecated. :pr:<code>4997</code></p>
</li>
<li>
<p>The <code>locked_cached_property</code> decorator is deprecated. Use a lock inside the
decorated function if locking is needed. :issue:<code>4993</code></p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/flask/commit/f3b8f570545200c87465d18386f3fc9f2258307a"><code>f3b8f57</code></a> release version 2.3.2</li>
<li><a href="https://github.com/pallets/flask/commit/c990bba94ab9bc81adf2d33e83c9a9628a2098f2"><code>c990bba</code></a> update min test env</li>
<li><a href="https://github.com/pallets/flask/commit/adedb2a64ea7703369bc89021710b439ee79f8dc"><code>adedb2a</code></a> Merge pull request <a href="https://redirect.github.com/pallets/flask/issues/5101">#5101</a> from pallets/update-werkzeug</li>
<li><a href="https://github.com/pallets/flask/commit/e1aedecdc689cc9a79131851dbdabf6c3bc49c9e"><code>e1aedec</code></a> update werkzeug</li>
<li><a href="https://github.com/pallets/flask/commit/37badc3ce8b0665e3454547839196a676729309f"><code>37badc3</code></a> update changelog</li>
<li><a href="https://github.com/pallets/flask/commit/70f906c51ce49c485f1d355703e9cc3386b1cc2b"><code>70f906c</code></a> Merge pull request from GHSA-m2qf-hxjv-5gpq</li>
<li><a href="https://github.com/pallets/flask/commit/8705dd39c4fa563ea0fe0bf84c85da8fcc98b88d"><code>8705dd3</code></a> set <code>Vary: Cookie</code> header consistently for session</li>
<li><a href="https://github.com/pallets/flask/commit/9532cba45d2339e90ebf04f178b1e4f2064e7328"><code>9532cba</code></a> fix mypy finding</li>
<li><a href="https://github.com/pallets/flask/commit/0bc7356ce1ae11e633426902aba76d525f4523da"><code>0bc7356</code></a> start version 2.3.2</li>
<li><a href="https://github.com/pallets/flask/commit/f07fb2b607c1eaa724ca9bfe43e2dc20d97d34de"><code>f07fb2b</code></a> Merge pull request <a href="https://redirect.github.com/pallets/flask/issues/5086">#5086</a> from pallets/release-2.3.1</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/flask/compare/2.0.1...2.3.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=flask&package-manager=pip&previous-version=2.0.1&new-version=2.3.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-01 23:11:52 +0000 UTC
    </div>
</div>

