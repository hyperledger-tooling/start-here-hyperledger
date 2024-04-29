---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    Reduce SP usage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-26 13:55:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    Update FSC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 15:37:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    get datasource from environment variable, fix panic on open db error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 13:51:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Fts crypto code refactoring
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                * Remove un-necessary crypto code. 
* Remove anonymous issuance for the time being. Replace it instead with `type_is_hidden` or `not`. In systems with a single issuer hiding the type can be required. For transparent accounting, systems may require the type to be revealed at issuance time. In systems where a single issuer issues a single type, the type is implicitly revealed. 
* We plan to support anonymous issuance if applications call for it. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 09:23:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/614" class=".btn">#614</a>
            </td>
            <td>
                <b>
                    query directly token requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 05:46:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    remove orion commit processor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does the following: It removes the orion transaction processor. Transactions are committed into the local databases upon an event received via a finality listener. 
Next step is to remove the fabric transaction processor too. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 04:14:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/612" class=".btn">#612</a>
            </td>
            <td>
                <b>
                    add ability to query for token details
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR:

- Adds the ability to query for token with details, to allow the user to enrich the data about a transaction
- Splits the Raw Owner into its two components for more efficient queries. This can later be extended to the Owner struct in the Token (replacing the raw version)
- Stores the ApplicationMetadata as a separate field of the token request and adds it to retrieved transactions (where they are usually used)
- Returns owners when doing GetToken
- Simplifies the code of the querybuilder a bit

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 09:39:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    register transaction filter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-24 04:25:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/610" class=".btn">#610</a>
            </td>
            <td>
                <b>
                    use interface for ScanForPreImage so it can be called outside of a view
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">improvements</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 18:45:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/609" class=".btn">#609</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 25.0.3+incompatible to 25.0.5+incompatible
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 25.0.3+incompatible to 25.0.5+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v25.0.5</h2>
<h2>25.0.5</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A25.0.5">docker/cli, 25.0.5 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A25.0.5">moby/moby, 25.0.5 milestone</a></li>
<li>Deprecated and removed features, see <a href="https://github.com/docker/cli/blob/v25.0.5/docs/deprecated.md">Deprecated Features</a>.</li>
<li>Changes to the Engine API, see <a href="https://github.com/moby/moby/blob/v25.0.5/docs/api/version-history.md">API version history</a>.</li>
</ul>
<h3>Security</h3>
<p>This release contains a security fix for <a href="https://github.com/moby/moby/security/advisories/GHSA-mq39-4gv4-mvpx">CVE-2024-29018</a>, a potential data exfiltration from 'internal' networks via authoritative DNS servers.</p>
<h3>Bug fixes and enhancements</h3>
<ul>
<li><a href="https://github.com/moby/moby/security/advisories/GHSA-mq39-4gv4-mvpx">CVE-2024-29018</a>: Do not forward requests to external DNS servers for a container that is only connected to an 'internal' network. Previously, requests were forwarded if the host's DNS server was running on a loopback address, like systemd's 127.0.0.53. <a href="https://redirect.github.com/moby/moby/pull/47589">moby/moby#47589</a></li>
<li>plugin: fix mounting /etc/hosts when running in UserNS. <a href="https://redirect.github.com/moby/moby/pull/47588">moby/moby#47588</a></li>
<li>rootless: fix <code>open /etc/docker/plugins: permission denied</code>. <a href="https://redirect.github.com/moby/moby/pull/47587">moby/moby#47587</a></li>
<li>Fix multiple parallel <code>docker build</code> runs leaking disk space. <a href="https://redirect.github.com/moby/moby/pull/47527">moby/moby#47527</a></li>
</ul>
<h2>v25.0.4</h2>
<h2>25.0.4</h2>
<p>For a full list of pull requests and changes in this release, refer to the relevant GitHub milestones:</p>
<ul>
<li><a href="https://github.com/docker/cli/issues?q=is%3Aclosed+milestone%3A25.0.4">docker/cli, 25.0.4 milestone</a></li>
<li><a href="https://github.com/moby/moby/issues?q=is%3Aclosed+milestone%3A25.0.4">moby/moby, 25.0.4 milestone</a></li>
<li>Deprecated and removed features, see <a href="https://github.com/docker/cli/blob/v25.0.4/docs/deprecated.md">Deprecated Features</a>.</li>
<li>Changes to the Engine API, see <a href="https://github.com/moby/moby/blob/v25.0.4/docs/api/version-history.md">API version history</a>.</li>
</ul>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>Restore DNS names for containers in the default &quot;nat&quot; network on Windows. <a href="https://redirect.github.com/moby/moby/pull/47490">moby/moby#47490</a></li>
<li>Fix <code>docker start</code> failing when used with <code>--checkpoint</code> <a href="https://redirect.github.com/moby/moby/pull/47466">moby/moby#47466</a></li>
<li>Don't enforce new validation rules for existing swarm networks <a href="https://redirect.github.com/moby/moby/pull/47482">moby/moby#47482</a></li>
<li>Restore IP connectivity between the host and containers on an internal bridge network. <a href="https://redirect.github.com/moby/moby/pull/47481">moby/moby#47481</a></li>
<li>Fix a regression introduced in v25.0 that prevented the classic builder from ADDing a tar archive with xattrs created on a non-Linux OS <a href="https://redirect.github.com/moby/moby/pull/47483">moby/moby#47483</a></li>
<li>containerd image store: Fix image pull not emitting <code>Pulling fs layer</code> status <a href="https://redirect.github.com/moby/moby/pull/47484">moby/moby#47484</a></li>
</ul>
<h3>API</h3>
<ul>
<li>To preserve backwards compatibility, make read-only mounts not recursive by default when using older clients (API version &lt; v1.44). <a href="https://redirect.github.com/moby/moby/pull/47393">moby/moby#47393</a></li>
<li><code>GET /images/{id}/json</code> omits the <code>Created</code> field (previously it was <code>0001-01-01T00:00:00Z</code>) if the <code>Created</code> field is missing from the image config. <a href="https://redirect.github.com/moby/moby/pull/47451">moby/moby#47451</a></li>
<li>Populate a missing <code>Created</code> field in <code>GET /images/{id}/json</code> with <code>0001-01-01T00:00:00Z</code> for API version &lt;= 1.43. <a href="https://redirect.github.com/moby/moby/pull/47387">moby/moby#47387</a></li>
<li>Fix a regression that caused API socket connection failures to report an API version negotiation failure instead. <a href="https://redirect.github.com/moby/moby/pull/47470">moby/moby#47470</a></li>
<li>Preserve supplied endpoint configuration in a container-create API request, when a container-wide MAC address is specified, but <code>NetworkMode</code> name-or-id is not the same as the name-or-id used in <code>NetworkSettings.Networks</code>. <a href="https://redirect.github.com/moby/moby/pull/47510">moby/moby#47510</a></li>
</ul>
<h3>Packaging updates</h3>
<ul>
<li>Upgrade Go runtime to <a href="https://go.dev/doc/devel/release#go1.21.8">1.21.8</a>. <a href="https://redirect.github.com/moby/moby/pull/47503">moby/moby#47503</a></li>
<li>Upgrade RootlessKit to <a href="https://github.com/rootless-containers/rootlesskit/releases/tag/v2.0.2">v2.0.2</a>.  <a href="https://redirect.github.com/moby/moby/pull/47508">moby/moby#47508</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/e63daec8672d77ac0b2b5c262ef525c7cf17fd20"><code>e63daec</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47589">#47589</a> from vvoland/v25.0-47538</li>
<li><a href="https://github.com/moby/moby/commit/817bccb1c65823f29eccf95b812ec9cf26da798c"><code>817bccb</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47588">#47588</a> from vvoland/v25.0-47558</li>
<li><a href="https://github.com/moby/moby/commit/2a0601e84e13514d7b94ab6687a33973eb0d80a0"><code>2a0601e</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47587">#47587</a> from vvoland/v25.0-47559</li>
<li><a href="https://github.com/moby/moby/commit/9df9ccc06fbcbb5ca9dc995f6075cc18341b3816"><code>9df9ccc</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/47586">#47586</a> from vvoland/v25.0-47569</li>
<li><a href="https://github.com/moby/moby/commit/a987bc5ad06c54448454b5415dd70465d41c184e"><code>a987bc5</code></a> libnet: Don't forward to upstream resolvers on internal nw</li>
<li><a href="https://github.com/moby/moby/commit/20c205fd3a0081d005958eff690e2b34df1c5e5e"><code>20c205f</code></a> Environment variable to override resolv.conf path.</li>
<li><a href="https://github.com/moby/moby/commit/4be97233cc191bda476d8ecfcd6ee48446ddb3da"><code>4be9723</code></a> daemon: move getUnprivilegedMountFlags to internal package</li>
<li><a href="https://github.com/moby/moby/commit/7ed7e6caf6c1605ba5fcc80c015b4afced7c8bfd"><code>7ed7e6c</code></a> plugin: fix mounting /etc/hosts when running in UserNS</li>
<li><a href="https://github.com/moby/moby/commit/81ad7062f0299c4ebc9ac3f576a2c0c67d8b6ff8"><code>81ad706</code></a> rootless: fix <code>open /etc/docker/plugins: permission denied</code></li>
<li><a href="https://github.com/moby/moby/commit/02d4ee3f9aea7e296ac3f3afb39d4428c38c6251"><code>02d4ee3</code></a> Makefile: generate-files: fix check for empty TMP_OUT</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v25.0.3...v25.0.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=25.0.3+incompatible&new-version=25.0.5+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-token-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 14:17:02 +0000 UTC
    </div>
</div>

