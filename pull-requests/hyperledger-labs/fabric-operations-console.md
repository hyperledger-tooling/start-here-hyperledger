---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/442" class=".btn">#442</a>
            </td>
            <td>
                <b>
                    add migration field on existing components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Add migration field to components on the original console.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 20:05:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/441" class=".btn">#441</a>
            </td>
            <td>
                <b>
                    conform "\"k8s\"" to "k8s" in cluster type api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Better parsing on the cluster type api to handle double quotes around the cluster type value. So this converts ` "\"k8s\""` to simply `"k8s"`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-10 19:38:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/440" class=".btn">#440</a>
            </td>
            <td>
                <b>
                    Fix timeouts & streamline requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
- conformed client timeouts to be used consistently, filled in some fabric calls that did not have custom timeouts
  - some timeout values for certain http requests have changed
- when checking a OS cluster for channel participation apis (aka osn admin features), the requests will now be sent in parallel 
- avoids sending back a 408 http code to the browser to prevent automatic retries, uses 504 instead
  - this dramatically improves performance on requests to non responsive endpoints
- lowered the number of retries for component status call requests
- increased the number of retries for component status call requests when components have just been created
- increased the interval on the client logs to store them less often, to minimize traffic

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 20:02:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/439" class=".btn">#439</a>
            </td>
            <td>
                <b>
                    fix node ou parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The node ou parsing was not consistent. Sometimes the code expected a string, other times boolean. Added a helper function to conform and handle both cases.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-07 16:17:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/438" class=".btn">#438</a>
            </td>
            <td>
                <b>
                    decompress docs before migration edits settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The migration code that edits the settings doc prior to migration needs to decompress the backup data first. otherwise the edits do not happen and the new console is thrown into shenanigans. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-06 19:14:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/437" class=".btn">#437</a>
            </td>
            <td>
                <b>
                    destroy session on change password
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
The login session will now be destroyed after changing a user password.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 19:51:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/436" class=".btn">#436</a>
            </td>
            <td>
                <b>
                    fix file permissons on the _backups folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Node user needs write permissions to the `_backups` folder


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-05 13:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/435" class=".btn">#435</a>
            </td>
            <td>
                <b>
                    Bump github.com/docker/docker from 20.10.12+incompatible to 20.10.24+incompatible in /packages/fabric-deployer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">go</span>
            </td>
            <td>
                Bumps [github.com/docker/docker](https://github.com/docker/docker) from 20.10.12+incompatible to 20.10.24+incompatible.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/docker/releases">github.com/docker/docker's releases</a>.</em></p>
<blockquote>
<h2>v20.10.24</h2>
<h2>20.10.24</h2>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>Fixed a number of issues that can cause Swarm encrypted overlay networks
to fail to uphold their guarantees, addressing <a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-28841">CVE-2023-28841</a>,
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-28840">CVE-2023-28840</a>, and
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-28842">CVE-2023-28842</a>.
<ul>
<li>A lack of kernel support for encrypted overlay networks now reports
as an error.</li>
<li>Encrypted overlay networks are eagerly set up, rather than waiting for
multiple nodes to attach.</li>
<li>Encrypted overlay networks are now usable on Red Hat Enterprise Linux 9
through the use of the <code>xt_bpf</code> kernel module.</li>
<li>Users of Swarm overlay networks should review <a href="https://github.com/moby/moby/security/advisories/GHSA-vwm3-crmr-xfxw">GHSA-vwm3-crmr-xfxw</a>
to ensure that unintentional exposure has not occurred.</li>
</ul>
</li>
<li>Upgrade github.com/containerd/fifo to v1.1.0 to fix a potential panic <a href="https://redirect.github.com/moby/moby/pull/45242">moby/moby#45216</a>.</li>
<li>Fix missing Bash completion for installed cli-plugins <a href="https://redirect.github.com/docker/cli/pull/4091">docker/cli#4091</a>.</li>
</ul>
<h3>Packaging Updates</h3>
<ul>
<li>Update Go runtime to <a href="https://go.dev/doc/devel/release#go1.19.minor">1.19.7</a>.</li>
<li>Update Docker Buildx to <a href="https://github.com/docker/buildx/releases/tag/v0.10.4">v0.10.4</a>.</li>
<li>Update containerd to <a href="https://github.com/containerd/containerd/releases/tag/v1.6.20">v1.6.20</a>.</li>
<li>Update runc to <a href="https://github.com/opencontainers/runc/releases/tag/v1.1.5">v1.1.5</a>.</li>
</ul>
<h2>v20.10.23</h2>
<h3>Bug fixes and enhancements</h3>
<ul>
<li>
<p>Fix an issue where <code>docker build</code> would fail when using <code>--add-host=host.docker.internal:host-gateway</code>
with BuildKit enabled <a href="https://redirect.github.com/moby/moby/pull/44650">moby/moby#44650</a>.</p>
</li>
<li>
<p>Revert seccomp: block socket calls to <code>AF_VSOCK</code> in default profile <a href="https://redirect.github.com/moby/moby/pull/44712">moby/moby#44712</a>.
This change, while favorable from a security standpoint, caused a change
in behavior for some use-cases. As such, we are reverting it to ensure
stability and compatibility for the affected users.</p>
<p>However, users of <code>AF_VSOCK</code> in containers should recognize that this
(special) address family is not currently namespaced in any version of
the Linux kernel, and may result in unexpected behavior, like containers
communicating directly with host hypervisors.</p>
<p>Future releases, will filter <code>AF_VSOCK</code>. Users who need to allow containers
to communicate over the unnamespaced <code>AF_VSOCK</code> will need to turn off seccomp
confinement or set a custom seccomp profile.</p>
</li>
</ul>
<h3>Packaging Updates</h3>
<ul>
<li>Update Docker Compose to <a href="https://github.com/docker/compose/releases/tag/v2.15.1">v2.15.1</a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/moby/moby/commit/5d6db842238e3c4f5f9fb9ad70ea46b35227d084"><code>5d6db84</code></a> Merge pull request from GHSA-232p-vwff-86mp</li>
<li><a href="https://github.com/moby/moby/commit/d2bc43a75b98887a830501211cc6bc86a59b8cca"><code>d2bc43a</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/45242">#45242</a> from neersighted/go1.19.7/20.10</li>
<li><a href="https://github.com/moby/moby/commit/9aa5d55a8ba8725133a6fbb5ac98d1fab341fdc7"><code>9aa5d55</code></a> update to go1.19.7</li>
<li><a href="https://github.com/moby/moby/commit/83679bb638b7d20c913019d62535228e5ed8a1ec"><code>83679bb</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/45216">#45216</a> from corhere/backport-20.10/containerd-fifo_v1.1</li>
<li><a href="https://github.com/moby/moby/commit/b4f0442da2d6f432df52ce60d571d512336bcbd9"><code>b4f0442</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/45219">#45219</a> from vvoland/test-windows-execstartfails-2010</li>
<li><a href="https://github.com/moby/moby/commit/ba043e86912d47ba760856cab9c34e8b294fe29d"><code>ba043e8</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/44990">#44990</a> from thaJeztah/20.10_backport_update_go1.19</li>
<li><a href="https://github.com/moby/moby/commit/b56fe595050578ced98af6c2deb70f3126cad0f9"><code>b56fe59</code></a> integration-cli: Enable TestExecStartFails on Windows</li>
<li><a href="https://github.com/moby/moby/commit/d9433ee0968c963bc1c993ad408b5da791340175"><code>d9433ee</code></a> Merge pull request <a href="https://redirect.github.com/docker/docker/issues/45197">#45197</a> from vvoland/integration-restart-race-2010</li>
<li><a href="https://github.com/moby/moby/commit/a9c02c238f403a7a204c909fe5f85fcef13faf75"><code>a9c02c2</code></a> Upgrade containerd/fifo to v1.1.0</li>
<li><a href="https://github.com/moby/moby/commit/bbec6704dcf31a981cec32e2ea95a6c19306a666"><code>bbec670</code></a> [20.10] vendor: libnetwork c5aa85f9b25f0acaec8591ced679cb9fb5b9e32c</li>
<li>Additional commits viewable in <a href="https://github.com/docker/docker/compare/v20.10.12...v20.10.24">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/docker/docker&package-manager=go_modules&previous-version=20.10.12+incompatible&new-version=20.10.24+incompatible)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-operations-console/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 21:15:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/434" class=".btn">#434</a>
            </td>
            <td>
                <b>
                    make couchdb url use ipv4 and not ipv6
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
With node 18, values of `localhost` are interpreted as their IPv6 equivalent of `::1`, however our couchdb containers are not listening on `::1`, they only work with IPv4. This PR replaces `localhost` on outgoing destinations with `127.0.0.1` to keep things as IPv4.

This fixes database connecting issues (with certain couchdb configurations) seen since build `1.0.5-3`.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-04 16:37:48 +0000 UTC
    </div>
</div>

