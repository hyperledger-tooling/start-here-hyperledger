---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1511" class=".btn">#1511</a>
            </td>
            <td>
                <b>
                    feat: oob without handhsake improvements and routing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Several improvements to the OOB and connection-less exchange flows.

Fixes #1376
Fixes #1250

Mainly it introduces the following changes:
- Integrate the legacy connection-less exchange with out of band, just like we do with the legacy connection invitations. This means that an out of band record will now be created when you call `createLegacyConnectionlessInvitation`. In addition, you can now also pass a legacy connectionless invitation url to `agent.oob.recieveInvitationFromUrl`. This will transform the legacy connectionless invitation to an out of band invitation. The method to receive the message using `agent.receiveMessage` works to not introduce breaking changes, but I've marked that method as deprecated and we can remove it in 0.5.0. This leaves multiple flows now that work, and we probably want to do some cleanup of the connectionless code once we remove the old flow in 0.5.0 (not using the oob api).
- The receiveInvitation already supported a `routing` prop, but this was not used for connection-less exchanges. This means you could not control which routing config would be used for a connection-less exchange you received an invitation for. Now the routing is used when you respond to a connectionless out of band invitation.
- Several bugs in the oob flow when using connectionless (this was broken).
- Added a `getOutboundMessageContext` method (again ;), we just removed it lol). But this takes into account everything that is needed for responding in connection-full and connection-less exchanges and removes a lot of the duplicated complex logic for handling connection-less. Once we remove the old flow (not using oob api, but still can use legacy connection-less), we could even fully abstract connection-less vs connection, and thus any protocol that uses the `DidCommMessageRepository` could support connection-less out of the box.

Our main use case for these changes is DIDComm over Bluetooth, where we use a mediator for normal HTTP exchagnes, but if we respond to an invitation over BLE, we want to use custom routing and explicitly set `useDefaultMediator` to false, so we can directly communicate over bluetooth instead of through a mediator.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 11:58:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1509" class=".btn">#1509</a>
            </td>
            <td>
                <b>
                    build(deps): bump word-wrap from 1.2.3 to 1.2.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [word-wrap](https://github.com/jonschlinkert/word-wrap) from 1.2.3 to 1.2.4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jonschlinkert/word-wrap/releases">word-wrap's releases</a>.</em></p>
<blockquote>
<h2>1.2.4</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove default indent by <a href="https://github.com/mohd-akram"><code>@​mohd-akram</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/24">jonschlinkert/word-wrap#24</a></li>
<li>🔒fix: CVE 2023 26115 (2) by <a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/41">jonschlinkert/word-wrap#41</a></li>
<li>:lock: fix: CVE-2023-26115 by <a href="https://github.com/aashutoshrathi"><code>@​aashutoshrathi</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/33">jonschlinkert/word-wrap#33</a></li>
<li>chore: publish workflow by <a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/42">jonschlinkert/word-wrap#42</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/mohd-akram"><code>@​mohd-akram</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/24">jonschlinkert/word-wrap#24</a></li>
<li><a href="https://github.com/OlafConijn"><code>@​OlafConijn</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/41">jonschlinkert/word-wrap#41</a></li>
<li><a href="https://github.com/aashutoshrathi"><code>@​aashutoshrathi</code></a> made their first contribution in <a href="https://redirect.github.com/jonschlinkert/word-wrap/pull/33">jonschlinkert/word-wrap#33</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.4">https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.4</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/f64b188c7261d26b99e1e2075d6b12f21798e83a"><code>f64b188</code></a> run verb to generate README</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/03ea08256ba0c8e8b02b1b304f0f5bd2b1863207"><code>03ea082</code></a> Merge pull request <a href="https://redirect.github.com/jonschlinkert/word-wrap/issues/42">#42</a> from jonschlinkert/chore/publish-workflow</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/420dce9a2412b21881202b73a3c34f0edc53cb2e"><code>420dce9</code></a> Merge pull request <a href="https://redirect.github.com/jonschlinkert/word-wrap/issues/41">#41</a> from jonschlinkert/fix/CVE-2023-26115-2</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/bfa694edf55bb84ff84512f13da6d68bf7593f06"><code>bfa694e</code></a> Update .github/workflows/publish.yml</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/ace0b3c78f81aaf43040bab3bc91d3c5546d3fd2"><code>ace0b3c</code></a> chore: bump version to 1.2.4</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/6fd727594676f3e1b196b08a320908bec2f4ca02"><code>6fd7275</code></a> chore: add publish workflow</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/30d6daf60fce429f5f559252fa86ee78200652c4"><code>30d6daf</code></a> chore: fix test</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/655929cabea6299dddf3b4a21fc3713fca701b48"><code>655929c</code></a> chore: remove package-lock</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/49e08bbc32a84da5d79e6b7e0fa74ff6217f6d81"><code>49e08bb</code></a> chore: added an additional testcase</li>
<li><a href="https://github.com/jonschlinkert/word-wrap/commit/9f626935f3fac6ec0f3c4b26baea4eb9740d9645"><code>9f62693</code></a> fix: cve 2023-26115</li>
<li>Additional commits viewable in <a href="https://github.com/jonschlinkert/word-wrap/compare/1.2.3...1.2.4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=word-wrap&package-manager=npm_and_yarn&previous-version=1.2.3&new-version=1.2.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 20:17:06 +0000 UTC
    </div>
</div>

