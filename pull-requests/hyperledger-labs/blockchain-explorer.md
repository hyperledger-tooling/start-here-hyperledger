---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/350" class=".btn">#350</a>
            </td>
            <td>
                <b>
                    added pagination for transactions view frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">do not merge</span>
            </td>
            <td>
                Signed-off-by: deekshithvarma256 <deekshithvarma256@email.com>

<!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
This feature integrates the Api calls to render server-side pagination for list of transactions to be fetched.
As of now the pagination is being handled from UI. Implementing pagination from backend addresses an issue when dealing with retrieval of huge data sets.
#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #347 

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

--> 
```release-note
Yes
```

#### Additional documentation, usage docs, etc.:

<!--
This section can be blank if this pull request does not require a release note.

When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.


-->
```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-13 06:55:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/349" class=".btn">#349</a>
            </td>
            <td>
                <b>
                    fix failing unit test cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it:
This PR has changeset for fixing the failing unit test cases

#### Which issue(s) this PR fixes:
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #336 

#### Special notes for your reviewer:
#339 can check test case status

#### Does this PR introduce a user-facing change?
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note
NONE
```

#### Additional documentation, usage docs, etc.:

<!--
This section can be blank if this pull request does not require a release note.

When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.


-->
```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-11 13:15:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/344" class=".btn">#344</a>
            </td>
            <td>
                <b>
                    Bump k8s.io/client-go from 0.16.8 to 0.20.0 in /app/platform/fabric/e2e-test/specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [k8s.io/client-go](https://github.com/kubernetes/client-go) from 0.16.8 to 0.20.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/kubernetes/client-go/commit/afa3b34fe368bbf3532c612f1d5abc45d0783c08"><code>afa3b34</code></a> Update dependencies to v0.20.0 tag</li>
<li><a href="https://github.com/kubernetes/client-go/commit/fb61a7c88cb9f599363919a34b7c54a605455ffc"><code>fb61a7c</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/kubernetes/client-go/issues/96720">#96720</a> from liggitt/throttled-logger</li>
<li><a href="https://github.com/kubernetes/client-go/commit/61471be615ffce3012bfe4e92d1ba70236960d90"><code>61471be</code></a> Deflake ThrottledLogger test</li>
<li><a href="https://github.com/kubernetes/client-go/commit/66db2540991da169fb60fce735064a55bfc52b71"><code>66db254</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/kubernetes/client-go/issues/95981">#95981</a> from caesarxuchao/http2-healthcheck</li>
<li><a href="https://github.com/kubernetes/client-go/commit/7c9ea22f769b83d7573af95555d7ff1423429003"><code>7c9ea22</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/kubernetes/client-go/issues/92743">#92743</a> from liggitt/gc</li>
<li><a href="https://github.com/kubernetes/client-go/commit/8dde295de4630e0b70c931e6386cce6bb0b5f579"><code>8dde295</code></a> Add a unit test testing the HTTP/2 health check help the REST client</li>
<li><a href="https://github.com/kubernetes/client-go/commit/c476b49dcfc420f1f2822f40ad82ef925f3f35cd"><code>c476b49</code></a> Add GC unit tests</li>
<li><a href="https://github.com/kubernetes/client-go/commit/77eda6a9395bd7884e99d484f29ae3c6d55f0eb9"><code>77eda6a</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/kubernetes/client-go/issues/96317">#96317</a> from Jefftree/test-ssa</li>
<li><a href="https://github.com/kubernetes/client-go/commit/76f48268c78c15fd661e8acc832daee49b40eed6"><code>76f4826</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/kubernetes/client-go/issues/96527">#96527</a> from adtac/apfbeta</li>
<li><a href="https://github.com/kubernetes/client-go/commit/4ab8fb4585a5873ae1c155d7f35c9710bd38f2d2"><code>4ab8fb4</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/kubernetes/client-go/issues/96425">#96425</a> from bobbypage/vendor-cadvisor-v0.38</li>
<li>Additional commits viewable in <a href="https://github.com/kubernetes/client-go/compare/v0.16.8...v0.20.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=k8s.io/client-go&package-manager=go_modules&previous-version=0.16.8&new-version=0.20.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-explorer/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 23:45:05 +0000 UTC
    </div>
</div>

