---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2840" class=".btn">#2840</a>
            </td>
            <td>
                <b>
                    Add anoncreds upgrade via api endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is WIP. More testing and refactoring.

This includes feature https://github.com/hyperledger/aries-cloudagent-python/pull/2822 as it was built off of it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-15 19:27:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2836" class=".btn">#2836</a>
            </td>
            <td>
                <b>
                    Remove requirement for write ledger in read-only mode.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #2829 

This change removes the requirement for the list of ledgers to specify at least a ledger with attribute `is_write` when running the agent in read-only mode.

I initially tried to mock the parsed argument in the tests as one was failing, however having attributes from different groups made mocking very complicated so I opted for moving this setting onto `LedgerGroup` as well, as it seems appropriate.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-14 01:16:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2835" class=".btn">#2835</a>
            </td>
            <td>
                <b>
                    feat: external suite provider interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a pluggable component enabling usage of an externally provided signature suite. This is a refinement on previous attempts to make this aspect of ACA-Py more flexible; namely, #2706 which was later reverted due to issues with including profile in the context and multi-tenancy. This approach minimizes the "surface area" of the interface that the plugin must fulfill (at least when compared to what was proposed in #2706).

This is an advanced use case requiring some fairly deep knowledge of the management of DIDs and VCs. I have an example implementation of using an external KMS for signing JSON-LD creds that I may push to the open as a starting point for interested parties.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-13 21:59:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2833" class=".btn">#2833</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jwcrypto from 1.5.4 to 1.5.6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jwcrypto](https://github.com/latchset/jwcrypto) from 1.5.4 to 1.5.6.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/latchset/jwcrypto/releases">jwcrypto's releases</a>.</em></p>
<blockquote>
<h2>Version 1.5.6 - Moderate Security release</h2>
<h2>What's Changed</h2>
<ul>
<li>Address potential DoS with high compression ratio by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/349">latchset/jwcrypto#349</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6">https://github.com/latchset/jwcrypto/compare/v1.5.5...v1.5.6</a></p>
<h2>Version 1.5.5</h2>
<p>This version fixes a pypi distribution problem introduced in 1.0 when pushing was automated.
With 1.5.5 a binary wheel is now also made available on pypi.</p>
<h2>What's Changed</h2>
<ul>
<li>Fix doc generation by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/345">latchset/jwcrypto#345</a></li>
<li>Update publish action to upload also binary dist by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/347">latchset/jwcrypto#347</a></li>
<li>Fix pypi publishing by <a href="https://github.com/simo5"><code>@​simo5</code></a> in <a href="https://redirect.github.com/latchset/jwcrypto/pull/348">latchset/jwcrypto#348</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5">https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.5</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/latchset/jwcrypto/commit/ecde4efdc7c9364b53bd1b4232e97557d821abdf"><code>ecde4ef</code></a> Version 1.5.6</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/90477a3b6e73da69740e00b8161f53fea19b831f"><code>90477a3</code></a> Address potential DoS with high compression ratio</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/240cc60fe4fe7458d3a7828c3e793795eb59a438"><code>240cc60</code></a> Modernize pypi action</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/491f4485562e94473e57bb9164eb290dcd3be3c5"><code>491f448</code></a> Version 1.5.5</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/7f51d28eea46f039ac363eaf348123394f17310c"><code>7f51d28</code></a> Update publish action to upload also binary dist</li>
<li><a href="https://github.com/latchset/jwcrypto/commit/5dc2ea2a87ea9fb3ed833f9f0f7864edc7b01e7b"><code>5dc2ea2</code></a> Fix doc generation</li>
<li>See full diff in <a href="https://github.com/latchset/jwcrypto/compare/v1.5.4...v1.5.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jwcrypto&package-manager=pip&previous-version=1.5.4&new-version=1.5.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-11 19:45:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2832" class=".btn">#2832</a>
            </td>
            <td>
                <b>
                    Create AnonCredsMethods.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Documentation for creating an AnonCreds Method.  Expands on document that @dbluhm presented the other day, and includes a link to the recording made of the discussion from Wednesday.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-10 04:27:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2831" class=".btn">#2831</a>
            </td>
            <td>
                <b>
                    Cleanup of docs, generator label fix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds the Traction Sandbox demo as well.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-09 17:00:00 +0000 UTC
    </div>
</div>

