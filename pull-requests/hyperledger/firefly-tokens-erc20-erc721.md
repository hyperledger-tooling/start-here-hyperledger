---
layout: default
title: firefly-tokens-erc20-erc721
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-tokens-erc20-erc721
---

# firefly-tokens-erc20-erc721 <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-tokens-erc20-erc721){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Patched Command Injection in lodash
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `lodash` versions prior to 4.17.21 are vulnerable to Command Injection via the template function.

**CVE-2021-23337**
`7.2/ 10`
CVSS:3.1/AV:N/AC:L/PR:H/UI:N/S:U/C:H/I:H/A:H

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 02:23:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Patch ProxyAgent vulnerable to MITM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
`Undici.ProxyAgent` never verifies the remote server's certificate, and always exposes all request & response data to the proxy. This unexpectedly means that proxies can MitM all HTTPS traffic, and if the proxy's URL is HTTP then it also means that nominally HTTPS requests are actually sent via plain-text HTTP between Undici and the proxy server.

## Impact
This affects all use of HTTPS via HTTP proxy using `Undici.ProxyAgent` with Undici or Node's global `fetch`. In this case, it removes all HTTPS security from all requests sent using Undici's `ProxyAgent`, allowing trivial MitM attacks by anybody on the network path between the client and the target server (local network users, your ISP, the proxy, the target server's ISP, etc).
This less seriously affects HTTPS via HTTPS proxies. When you send HTTPS via a proxy to a remote server, the proxy can freely view or modify all HTTPS traffic unexpectedly (but only the proxy).

**CVE-2022-32210**
`7.7/ 10`
CVSS:3.1/AV:N/AC:H/PR:H/UI:N/S:C/C:H/I:H/A:N

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 02:13:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/79" class=".btn">#79</a>
            </td>
            <td>
                <b>
                    🐛 BUG: Patched CVE-2022-24434 Crash in HeaderParser in dicer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This affects all versions of package dicer. A malicious attacker can send a modified form to server, and crash the nodejs service. A complete denial of service can be achived by sending the malicious form in a loop.

**CVE-2022-24434**
`7.5/ 10`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-16 02:10:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    fixing url manipulation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Equivalent of https://github.com/hyperledger/firefly-tokens-erc1155/pull/90

Fixing errors caused by URL manipulation logic described in https://github.com/hyperledger/firefly-tokens-erc1155/issues/53

Signed-off-by: Chengxuan Xing <chengxuan.xing@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-15 12:40:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    Pass through EthConnect/EVMConnect receipts unchanged
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Per https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/72#issuecomment-1210782114
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 19:47:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    OpenZeppelin Contracts's SignatureChecker may revert on invalid EIP-1271 signers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ``SignatureChecker.isValidSignatureNow`` is not expected to revert. However, an incorrect assumption about Solidity 0.8's ``abi.decode`` allows some cases to revert, given a target contract that doesn't implement EIP-1271 as expected.

The contracts that may be affected are those that use ``SignatureChecker`` to check the validity of a signature and handle invalid signatures in a way other than reverting. We believe this to be unlikely.

## Patches
The issue was patched in 4.7.1.

## References
https://github.com/OpenZeppelin/openzeppelin-contracts/pull/3552


## Additional Information
Please invited my github to contributed/collaborate at your project community.
Regards,
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 15:30:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    Bump simple-get from 2.8.1 to 2.8.2 in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [simple-get](https://github.com/feross/simple-get) from 2.8.1 to 2.8.2.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/feross/simple-get/commit/4e156b6bb19e11ccfad05fad310ea799d63f890d"><code>4e156b6</code></a> 2.8.2</li>
<li><a href="https://github.com/feross/simple-get/commit/43c272db3e4b1383cb03d80338dba3e08c451641"><code>43c272d</code></a> Bug fix: Thirdparty cookie leak</li>
<li>See full diff in <a href="https://github.com/feross/simple-get/compare/v2.8.1...v2.8.2">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~linusu">linusu</a>, a new releaser for simple-get since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=simple-get&package-manager=npm_and_yarn&previous-version=2.8.1&new-version=2.8.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-tokens-erc20-erc721/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 11:19:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    Bump minimist from 1.2.5 to 1.2.6 in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [minimist](https://github.com/substack/minimist) from 1.2.5 to 1.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/substack/minimist/commit/7efb22a518b53b06f5b02a1038a88bd6290c2846"><code>7efb22a</code></a> 1.2.6</li>
<li><a href="https://github.com/substack/minimist/commit/ef88b9325f77b5ee643ccfc97e2ebda577e4c4e2"><code>ef88b93</code></a> security notice for additional prototype pollution issue</li>
<li><a href="https://github.com/substack/minimist/commit/c2b981977fa834b223b408cfb860f933c9811e4d"><code>c2b9819</code></a> isConstructorOrProto adapted from PR</li>
<li><a href="https://github.com/substack/minimist/commit/bc8ecee43875261f4f17eb20b1243d3ed15e70eb"><code>bc8ecee</code></a> test from prototype pollution PR</li>
<li>See full diff in <a href="https://github.com/substack/minimist/compare/1.2.5...1.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=minimist&package-manager=npm_and_yarn&previous-version=1.2.5&new-version=1.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-tokens-erc20-erc721/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 11:18:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-tokens-erc20-erc721/pull/73" class=".btn">#73</a>
            </td>
            <td>
                <b>
                    Bump cross-fetch from 2.2.3 to 2.2.6 in /samples/solidity
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [cross-fetch](https://github.com/lquixada/cross-fetch) from 2.2.3 to 2.2.6.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/lquixada/cross-fetch/commit/bfe5fe2d9c64fe96e69e21f4d71c8260e4dca563"><code>bfe5fe2</code></a> 2.2.6</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/1a89b6607ecbc14e3180426bdf4f0512dd990bec"><code>1a89b66</code></a> added caret range to whatwg-fetch.</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/695a888532403e71d5ee9ba43e00c0aac4b9660d"><code>695a888</code></a> removed and disabled package-lock.json.</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/eac6c00e9b24fec78475b15c2c3af44d1e454c31"><code>eac6c00</code></a> Update away from vulnerable version of node-fetch (<a href="https://github-redirect.dependabot.com/lquixada/cross-fetch/issues/135">#135</a>)</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/3abdc676d0b198e54d87c0df17b59668243826c4"><code>3abdc67</code></a> 2.2.5</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/982e107bd15c677996af066c5d7a2320c5c4b8ae"><code>982e107</code></a> Locked node-fetch version.</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/0820407fd41fd26cb9b9937ae55f96eaabde1a5c"><code>0820407</code></a> 2.2.4</li>
<li><a href="https://github.com/lquixada/cross-fetch/commit/19fec4e9af220a8628cffe0249aab8fb094c5a7a"><code>19fec4e</code></a> Fixed vulnerability CVE-2020-15168 by upgrading node-fetch to 2.6.1.</li>
<li>See full diff in <a href="https://github.com/lquixada/cross-fetch/compare/v2.2.3...v2.2.6">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cross-fetch&package-manager=npm_and_yarn&previous-version=2.2.3&new-version=2.2.6)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/firefly-tokens-erc20-erc721/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 11:18:39 +0000 UTC
    </div>
</div>

