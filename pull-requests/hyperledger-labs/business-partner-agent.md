---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    w3c interoperability fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Testing connection and credential protocols against aries-framework-go.

**Fixes:**

- added option to create oob invitations with did:key
- prefixing peer did's with did:peer
- added aca-py's config flags that switch the didcomm mime-type as the wire format is not supported by the go-agent

**Tested:**
- [x] Receive/create oob invitations with did:key works both ways bpa <-> framework-go
- [ ] Receive/create did-exchange invitation - is not working with aca-py as only did:indy is supported
- [ ] Issue/receive w3c credentials

**Go Agent Config in IDE**

Start flags:

```
start --api-host localhost:8081 \
     --database-type mem \
     --inbound-host http@<host-ip>:8082 \
     --inbound-host-external http@http://<host-ip>:8082
     --webhook-url http://<host-ip>:8080/log
     --log-level DEBUG 
     --agent-default-label MyGoAgent
```
Compiler flags:

```
-tags ACAPyInterop
```
Environment:
```
ARIESD_AUTO_ACCEPT=true
```

**Curl against go-agent**

Create did-exchange invitation
```
 curl  -X 'POST' \
  'http://localhost:8081/connections/create-invitation' \
  -H 'accept: application/json' \
  -d ''
```

Create oob invitation:
```
curl -X 'POST' \
  'http://localhost:8081/outofband/create-invitation' \
  -H 'accept: application/json' \
  -H 'Content-Type: application/json' \
  -d '{"label": "Go Agent"}'
```

Receive oob invitation:
```
curl -X POST "http://localhost:8081/outofband/accept-invitation" -H  "content-type: application/json" -d "{\"invitation\":{\"@id\":\"5fa6dc8e-63ed-4af8-ae32-2533c109ea47\",\"@type\":\"https://didcomm.org/out-of-band/1.0/invitation\",\"services\":[{\"id\":\"#inline\",\"type\":\"did-communication\",\"recipientKeys\":[\"did:key:z6MkjHKsXMwNbn1xjG3ge2WWT1Gq7FLeCo2sgRqW5pVgjqdn\"],\"serviceEndpoint\":\"http://<host-ip>:8888\"}],\"handshake_protocols\":[\"https://didcomm.org/didexchange/1.0\"]},\"my_label\": \"aca-py\"}"
```

Get connections
```
curl -X GET "http://localhost:8081/connections" -H  "accept: application/json"
```

Test if connecting to the transport works
```
curl -v -X 'POST' -H 'Content-Type: application/didcomm-envelope-enc'  http://:<host-ip>:8082
```

Signed-off-by: Philipp Etschel <philipp.etschel@ch.bosch.com>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/718"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 11:41:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/717" class=".btn">#717</a>
            </td>
            <td>
                <b>
                    Bump url-parse from 1.5.3 to 1.5.7 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [url-parse](https://github.com/unshiftio/url-parse) from 1.5.3 to 1.5.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/unshiftio/url-parse/commit/8b3f5f2c88a4cfc2880f2319c307994cb25bb10a"><code>8b3f5f2</code></a> 1.5.7</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/ef45a1355375a8244063793a19059b4f62fc8788"><code>ef45a13</code></a> [fix] Readd the empty userinfo to <code>url.href</code> (<a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/226">#226</a>)</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/88df2346855f70cec9713b362ca32a4691dc271a"><code>88df234</code></a> [doc] Add soft deprecation notice</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/78e9f2f41285d83e7d91706be5bd439656fe3bc3"><code>78e9f2f</code></a> [security] Fix nits</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/e6fa43422c52f34c73146552ec9916125dc59525"><code>e6fa434</code></a> [security] Add credits for incorrect handling of userinfo vulnerability</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/4c9fa234c01dca52698666378360ad2fdfb05470"><code>4c9fa23</code></a> 1.5.6</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/7b0b8a6671f806458e88b1f44feb0fdd742cdf06"><code>7b0b8a6</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/unshiftio/url-parse/issues/223">#223</a> from unshiftio/fix/at-sign-handling-in-userinfo</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/e4a5807d95b971577e4d888f5b99d64a40851386"><code>e4a5807</code></a> 1.5.5</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/193b44baf3d203560735e05eedc99d8244c9e16c"><code>193b44b</code></a> [minor] Simplify whitespace regex</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/319851bf1c294796fc73e29ff31b14d9084e4a0d"><code>319851b</code></a> [fix] Remove CR, HT, and LF</li>
<li>Additional commits viewable in <a href="https://github.com/unshiftio/url-parse/compare/1.5.3...1.5.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url-parse&package-manager=npm_and_yarn&previous-version=1.5.3&new-version=1.5.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/717"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-19 12:45:18 +0000 UTC
    </div>
</div>

