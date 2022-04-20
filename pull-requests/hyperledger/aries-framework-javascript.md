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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/714" class=".btn">#714</a>
            </td>
            <td>
                <b>
                    feat: support handling messages with lower minor version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for processing messages with a lower minor version.

Some notes about the changes:
- The static `type` property on the message classes are now `ParsedMessageType` containing info about the message type. I've done this to make the info readily available and not have to parse it every time we need this info (would need to be done for every message for each message received). This is how declaring the type now looks. `praseMessageType` is an utitliy method that makes it easier to created the `ParsedMessageType` object.
```ts
class CustomProtocolMessage extends AgentMessage {
  @IsValidMessageType(CustomProtocolMessage.type)
  public readonly type = CustomProtocolMessage.type.messageTypeUri
  public static readonly type = parseMessageType('https://didcomm.org/fake-protocol/1.5/message')
}
```
- Had to refactor the decorators a bit as it was incorrectly typed which was now causing errors with typescript
- Added an e2e test where we send a message with a lower minor version to another agent with a higher minor version.
- Added transformations from string values `1` and `0` to `n__1` and `n__0`. See here for the relevant discussion: https://github.com/hyperledger/aries-framework-javascript/pull/690#discussion_r850942240. Other approaches very welcome.

This PR doesn't include handling the error case where we receive a message with a higher minor version. I'll like to address that in a separate PR (should be straightforward, we just have to change the reason in the problem report), but this at least unblocks us now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 10:49:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/712" class=".btn">#712</a>
            </td>
            <td>
                <b>
                    fix: allow agent without inbound endpoint to connect when using multi-use invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Quite an edge case, but when an agent without an inbound endpoint (e.g. mobile wallet connecting to mediator) would respond to a multi-use connection invitation (quite common with mediators) the session would be stored for the multi-use invitation connection. But during the processing of the request a new connection will be created, which means the session won't be reused afterwards because it's tied to the multi-use invitation connection. 

Normally this isn't that big a deal, as the next time a message is sent using the new connection the session can be reused, but for agent without an inbound transport this made it impossible to connect to AFJ. 

This PR adds the sessionId to the inbound message, and later attaches it to the outbound message. This is only used when directly responding to an incoming message. Wasn't sure if attaching the sessionId is the best here, but couldn't think of other straightforward approaches. We basically want to attach it to the inbound message, so we can just respond to the inbound session (instead of finding a session by the connection id, which is still used for a lot of other use cases)

Also changed the subject transport a bit to not require an inbound transport anymore when no inbound endpoint is configured (better reflects real-world setup)

Fixes #483 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 21:57:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/711" class=".btn">#711</a>
            </td>
            <td>
                <b>
                    feat: pickup v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implemented [pickup v2 protocol ](https://github.com/hyperledger/aries-rfcs/tree/main/features/0685-pickup-v2#delivery-request) along with unit testing for the implemented methods leaving room for future testing within the Mediation Recipient Module. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-15 21:57:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/710" class=".btn">#710</a>
            </td>
            <td>
                <b>
                    build(deps): bump async from 2.6.3 to 2.6.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [async](https://github.com/caolan/async) from 2.6.3 to 2.6.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/caolan/async/blob/v2.6.4/CHANGELOG.md">async's changelog</a>.</em></p>
<blockquote>
<h1>v2.6.4</h1>
<ul>
<li>Fix potential prototype pollution exploit (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1828">#1828</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/caolan/async/commit/c6bdaca4f9175c14fc655d3783c6af6a883e6514"><code>c6bdaca</code></a> Version 2.6.4</li>
<li><a href="https://github.com/caolan/async/commit/8870da9d5022bab310413041b4079e10db3980b7"><code>8870da9</code></a> Update built files</li>
<li><a href="https://github.com/caolan/async/commit/4df6754ef4e96a742956df8782fee27242a2ea12"><code>4df6754</code></a> update changelog</li>
<li><a href="https://github.com/caolan/async/commit/8f7f90342a6571ba1c197d747ebed30c368096d2"><code>8f7f903</code></a> Fix prototype pollution vulnerability (<a href="https://github-redirect.dependabot.com/caolan/async/issues/1828">#1828</a>)</li>
<li>See full diff in <a href="https://github.com/caolan/async/compare/v2.6.3...v2.6.4">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~hargasinski">hargasinski</a>, a new releaser for async since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async&package-manager=npm_and_yarn&previous-version=2.6.3&new-version=2.6.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
Dependabot will merge this PR once CI passes on it, as requested by @TimoGlastra.

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-14 19:04:44 +0000 UTC
    </div>
</div>

