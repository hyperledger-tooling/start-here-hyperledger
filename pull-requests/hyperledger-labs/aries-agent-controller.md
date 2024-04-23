---
layout: default
title: aries-agent-controller
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/aries-agent-controller
---

# aries-agent-controller <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/aries-agent-controller){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aries-agent-controller/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Bump gunicorn from 20.1.0 to 22.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [gunicorn](https://github.com/benoitc/gunicorn) from 20.1.0 to 22.0.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/benoitc/gunicorn/releases">gunicorn's releases</a>.</em></p>
<blockquote>
<h2>Gunicorn 22.0 has been released</h2>
<p><strong>Gunicorn 22.0.0 has been released.</strong> This version fix the numerous security vulnerabilities. You're invited to upgrade asap your own installation.</p>
<p>Changes:</p>
<pre><code>22.0.0 - 2024-04-17
===================
<ul>
<li>use <code>utime</code> to notify workers liveness</li>
<li>migrate setup to pyproject.toml</li>
<li>fix numerous security vulnerabilities in HTTP parser (closing some request smuggling vectors)</li>
<li>parsing additional requests is no longer attempted past unsupported request framing</li>
<li>on HTTP versions &lt; 1.1 support for chunked transfer is refused (only used in exploits)</li>
<li>requests conflicting configured or passed SCRIPT_NAME now produce a verbose error</li>
<li>Trailer fields are no longer inspected for headers indicating secure scheme</li>
<li>support Python 3.12</li>
</ul>
<p>** Breaking changes **</p>
<ul>
<li>minimum version is Python 3.7</li>
<li>the limitations on valid characters in the HTTP method have been bounded to Internet Standards</li>
<li>requests specifying unsupported transfer coding (order) are refused by default (rare)</li>
<li>HTTP methods are no longer casefolded by default (IANA method registry contains none affected)</li>
<li>HTTP methods containing the number sign (#) are no longer accepted by default (rare)</li>
<li>HTTP versions &lt; 1.0 or &gt;= 2.0 are no longer accepted by default (rare, only HTTP/1.1 is supported)</li>
<li>HTTP versions consisting of multiple digits or containing a prefix/suffix are no longer accepted</li>
<li>HTTP header field names Gunicorn cannot safely map to variables are silently dropped, as in other software</li>
<li>HTTP headers with empty field name are refused by default (no legitimate use cases, used in exploits)</li>
<li>requests with both Transfer-Encoding and Content-Length are refused by default (such a message might indicate an attempt to perform request smuggling)</li>
<li>empty transfer codings are no longer permitted (reportedly seen with really old &amp; broken proxies)</li>
</ul>
<p>** SECURITY **</p>
<ul>
<li>fix CVE-2024-1135
</code></pre></li>
</ul>
<ol>
<li>Documentation is available there: <a href="https://docs.gunicorn.org/en/stable/news.html">https://docs.gunicorn.org/en/stable/news.html</a></li>
<li>Packages: <a href="https://pypi.org/project/gunicorn/">https://pypi.org/project/gunicorn/</a></li>
</ol>
<h2>Gunicorn 21.2.0 has been released</h2>
<p><strong>Gunicorn 21.2.0 has been released.</strong> This version fix the issue introduced in the threaded worker.</p>
<p>Changes:</p>
<pre><code>21.2.0 - 2023-07-19
===================
fix thread worker: revert change considering connection as idle .
&lt;/tr&gt;&lt;/table&gt; 
</code></pre>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/benoitc/gunicorn/commit/f63d59e4d73a8ee28748d2c700fb81c8780bc419"><code>f63d59e</code></a> bump to 22.0</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/4ac81e0a1037ba5b570323be7430e09caa233e38"><code>4ac81e0</code></a> Merge pull request <a href="https://redirect.github.com/benoitc/gunicorn/issues/3175">#3175</a> from e-kwsm/typo</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/401cecfaed85d79236c7a9a1f7d8946b01c466fc"><code>401cecf</code></a> Merge pull request <a href="https://redirect.github.com/benoitc/gunicorn/issues/3179">#3179</a> from dhdaines/exclude-eventlet-0360</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/0243ec39ef4fc1b479ff4e1659e165f0b980b571"><code>0243ec3</code></a> fix(deps): exclude eventlet 0.36.0</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/628a0bcb61ef3a211d67dfd68ad1ba161cccb3b8"><code>628a0bc</code></a> chore: fix typos</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/88fc4a43152039c28096c8ba3eeadb3fbaa4aff9"><code>88fc4a4</code></a> Merge pull request <a href="https://redirect.github.com/benoitc/gunicorn/issues/3131">#3131</a> from pajod/patch-py12-rebased</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/deae2fc4c5f93bfce59be5363055d4cd4ab1b0b6"><code>deae2fc</code></a> CI: back off the agressive timeout</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/f4703824c323fe6867dce0e2f11013b8de319353"><code>f470382</code></a> docs: promise 3.12 compat</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/5e30bfa6b1a3e1f2bde7feb514d1734d28f39231"><code>5e30bfa</code></a> add changelog to project.urls (updated for PEP621)</li>
<li><a href="https://github.com/benoitc/gunicorn/commit/481c3f9522edc58806a3efc5b49be4f202cc7700"><code>481c3f9</code></a> remove setup.cfg - overridden by pyproject.toml</li>
<li>Additional commits viewable in <a href="https://github.com/benoitc/gunicorn/compare/20.1.0...22.0.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gunicorn&package-manager=pip&previous-version=20.1.0&new-version=22.0.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/aries-agent-controller/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 02:21:54 +0000 UTC
    </div>
</div>

